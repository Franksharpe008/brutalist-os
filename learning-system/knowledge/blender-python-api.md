# BLENDER PYTHON API KNOWLEDGE BASE
# Everything I know about Blender automation via Python

Last updated: 2026-02-18
Source: Official docs, CG Cookie, Blender Stack Exchange

---

## CORE CONCEPTS

### bpy Module
**What it is:** Blender's Python API module

**Key entry points:**
```python
import bpy  # Main module

# Object operations
bpy.ops.mesh.primitive_*_add()    # Create geometry
bpy.ops.object.*                 # Manipulate objects
bpy.ops.material.*                # Create materials
bpy.ops.render.*                # Control rendering

# Data access
bpy.data.objects                   # All objects
bpy.data.materials                 # All materials
bpy.data.cameras                   # All cameras
bpy.context.scene                  # Current scene
```

### Context Management
**Critical concept:** Blender requires active context

```python
# BAD - will fail if nothing selected
bpy.ops.object.delete()  # Error: context is incorrect

# GOOD - ensure context
if bpy.context.active_object:
    bpy.ops.object.delete()

# BEST - set context explicitly
bpy.context.view_layer.objects.active = obj
bpy.ops.object.delete()
```

---

## GEOMETRY CREATION

### Primitive Shapes
```python
# Cube
bpy.ops.mesh.primitive_cube_add(size=2, location=(0,0,0))

# Sphere (UV sphere)
bpy.ops.mesh.primitive_uv_sphere_add(radius=1, location=(0,0,0))

# Plane
bpy.ops.mesh.primitive_plane_add(size=4, location=(0,0,0))

# Cylinder
bpy.ops.mesh.primitive_cylinder_add(radius=1, depth=2, location=(0,0,0))

# Monkey ( Suzanne )
bpy.ops.mesh.primitive_monkey_add(location=(0,0,0))
```

### Custom Geometry from Vertices
```python
mesh = bpy.data.meshes.new("MyMesh", "OBJECT")
obj = bpy.data.objects.new("MyObject", mesh)
bpy.context.collection.objects.link(obj)

# Add vertices and edges
mesh.from_pydata(vertices, [], edges, [])
```

---

## MATERIALS & SHADERS

### Principled BSDF (Modern PBR)
```python
mat = bpy.data.materials.new(name="MyMaterial")
mat.use_nodes = True
nodes = mat.node_tree.nodes
links = mat.node_tree.links

# Get standard setup
bsdf = nodes.get("Principled BSDF")
bsdf.inputs['Base Color'].default_value = (0.8, 0.2, 0.1, 1)  # RGBA
bsdf.inputs['Metallic'].default_value = 0.5
bsdf.inputs['Roughness'].default_value = 0.3
bsdf.inputs['IOR'].default_value = 1.5

# Apply to object
obj.data.materials.append(mat)
```

### Procedural Textures (No image files needed)
```python
# Noise texture
tex = nodes.new(type='ShaderNodeTexNoise')
tex.inputs['Scale'].default_value = 5.0

# Voronoi texture
tex = nodes.new(type='ShaderNodeTexVoronoi')
tex.inputs['Scale'].default_value = 3.0

# Map to material
links.new(tex.outputs['Color'], bsdf.inputs['Base Color'])
```

---

## LIGHTING

### Light Types
```python
# Sun light (directional)
bpy.ops.object.light_add(type='SUN', location=(5,5,5))

# Point light (omnidirectional)
bpy.ops.object.light_add(type='POINT', location=(0,0,5))
bpy.context.active_object.data.energy = 1000

# Spot light
bpy.ops.object.light_add(type='SPOT', location=(0,5,5))
```

### HDRI Environment Lighting
```python
world = bpy.context.scene.world
world.use_nodes = True
node_tree = world.node_tree

bg = node_tree.nodes['Background']
env = node_tree.nodes.new('ShaderNodeTexEnvironment')

# Load HDR image (needs file in assets/)
env.image = bpy.data.images.load('path/to/studio.hdr')

node_tree.links.new(env.outputs['Color'], bg.inputs['Color'])
```

---

## CAMERA CONTROL

### Create & Position
```python
# Create camera data
cam_data = bpy.data.cameras.new("MyCamera")

# Create camera object
cam_obj = bpy.data.objects.new("MyCamera", cam_data)
bpy.context.collection.objects.link(cam_obj)

# Position
cam_obj.location = (5, -5, 3)

# Rotation (in radians)
import math
cam_obj.rotation_euler = (math.radians(60), 0, math.radians(45))

# Set active
bpy.context.scene.camera = cam_obj
```

### Render Settings
```python
# Engine
bpy.context.scene.render.engine = 'BLENDER_EEVEE_NEXT'  # For Blender 4.x
# Older: bpy.context.scene.render.engine = 'CYCLES'

# Resolution
bpy.context.scene.render.resolution_x = 1920
bpy.context.scene.render.resolution_y = 1080

# File output
bpy.context.scene.render.filepath = '/tmp/output.png'
bpy.context.scene.render.image_settings.file_format = 'PNG'

# Render
bpy.ops.render.render(write_still=True)
```

---

## EXPORT FORMATS

### GLB/GLTF (Web-ready 3D)
```python
# Set export settings
bpy.ops.export_scene.gltf(
    filepath='model.glb',
    export_selected=True,
    export_format='GLB',
    use_selection=True,
    export_texcoords=True,
    export_normals=True,
    export_materials='EXPORT'
)
```

### OBJ (Classic 3D)
```python
bpy.ops.export_scene.obj(
    filepath='model.obj',
    use_selection=True,
    export_normals=True,
    export_uv=True
)
```

---

## COMMON ERRORS & SOLUTIONS

### Error: "context is incorrect"
**Cause:** Trying to operate on object that's not in context

**Solution:**
```python
# Set object as active
bpy.context.view_layer.objects.active = obj

# Or ensure object exists
if obj in bpy.context.view_layer.objects:
    bpy.ops.object.delete()
```

### Error: enum "BLENDER_EEVEE" not found
**Cause:** Old render engine name

**Solution:**
```python
# For Blender 4.x
bpy.context.scene.render.engine = 'BLENDER_EEVEE_NEXT'

# Not 'BLENDER_EEVEE' (typo in my first attempt)
```

### Error: Mesh has no geometry
**Cause:** Creating mesh from empty data

**Solution:**
```python
# Must provide vertices
mesh.from_pydata(vertices, [], [])

# Or use primitives (they have geometry)
bpy.ops.mesh.primitive_cube_add()
```

---

## ANIMATION BASICS

### Keyframe Insertion
```python
# Move object to X position
obj.location.x = 5
obj.keyframe_insert(data_path="location", frame=1)

# Move to Y position at frame 30
obj.location.y = 2
obj.keyframe_insert(data_path="location", frame=30)

# Animate 1-30
bpy.context.scene.frame_start = 1
bpy.context.scene.frame_end = 30
bpy.ops.render.render(animation=True)
```

### Rigging Constraints
```python
# Parent constraint
constraint = obj.constraints.new(type='COPY_LOCATION')
constraint.target = target_obj

# Track constraint
constraint = obj.constraints.new(type='TRACK_TO')
constraint.target = camera_obj
```

---

## PERFORMANCE OPTIMIZATION

### Reduce Polygon Count
```python
# Decimate modifier
mod = obj.modifiers.new(name="Decimate", type='DECIMATE')
mod.ratio = 0.5  # Reduce by 50%
```

### Optimize for Web (GLB)
```python
bpy.ops.export_scene.gltf(
    filepath='optimized.glb',
    export_format='GLB',
    export_apply_modifiers=True,  # Apply decimate
    export_tangents=True,         # Better shading
    export_colors=True
)
```

---

## MCP INTEGRATION

### When Using Blender MCP Addon
1. Install addon.py in Blender Preferences
2. Enable "MCP Blender Bridge"
3. Provide API key (e.g., Hyper3D)
4. Claude can send commands directly
5. Real-time control without manual Python

### Typical MCP Commands
```
"Create a sphere with glass material"
"Apply noise texture to selected object"
"Export current scene as GLB"
"Set lighting to studio setup"
```

---

## CROSS-REFERENCES

**Related to:**
- → Python scripting (general)
- → GLB export (web formats)
- → Three.js (web viewer)
- → Material nodes (procedural generation)
- → MCP protocols (automation)

**Used in projects:**
- Freestyle 3D Web Experience (2026-02-18)
- Automated asset generation pipeline (planned)
