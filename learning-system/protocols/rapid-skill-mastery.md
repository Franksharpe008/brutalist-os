# RAPID SKILL MASTERY PROTOCOL
# Step-by-step method for acquiring new capabilities efficiently

## Overview
Turn unknown → expert in 2-4 hours through structured learning

---

## Phase 1: Deep Research (30-45 minutes)

### What to Research
- [ ] Official documentation (primary source)
- [ ] Community best practices (GitHub, Stack Overflow, forums)
- [ ] Example implementations (real-world code)
- [ ] Common pitfalls and gotchas

### Research Questions to Answer
- What problem does this solve?
- What are the core concepts?
- What are the edge cases where it fails?
- How does it integrate with existing skills?
- What does "good" look like?

### Output
- Research summary document
- Working example from docs
- List of questions for testing
- Integration notes with current skill stack

---

## Phase 2: Prototype (30-45 minutes)

### Build Something Real
- [ ] Minimal viable implementation
- [ ] Test basic functionality
- [ ] Break it intentionally (find edge cases)
- [ ] Document what breaks

### Success Criteria
```
□ Runs without errors
□ Produces expected output
□ Handles 2+ edge cases
□ Can explain how it works
```

---

## Phase 3: Edge Case Testing (30-45 minutes)

### Push Boundaries
- [ ] Test with maximum input size
- [ ] Test with minimum/edge values
- [ ] Test with invalid data
- [ ] Test performance limits
- [ ] Test error handling

### Document Failures
For each failure found:
```
Input: [what caused it]
Expected: [what should happen]
Actual: [what happened]
Fix: [how to handle it]
```

---

## Phase 4: System Integration (15-30 minutes)

### Make It Part of Me
- [ ] Add to SKILL.md (if external skill)
- [ ] Update upgrade.yaml (proficiency +1)
- [ ] Create recall shortcut (link related concepts)
- [ ] Document typical use cases
- [ ] Build reusable wrapper/function

### Integration Checklist
```
□ Can I access it without looking up?
□ Does it work with other skills?
□ Is it indexed for instant recall?
□ Is there a working example in memory?
```

---

## Phase 5: Document for Recall (15 minutes)

### Cement Knowledge
- [ ] Write usage guide in plain language
- [ ] Add code snippets (copy-paste ready)
- [ ] Link to similar skills
- [ ] Note what it's NOT good for
- [ ] Update mastery timeline

---

## COMPOUNDING TRIGGERS

### When This Skill Unlocks Others
Document immediately in upgrade.yaml:
```yaml
unlocks_adjacent_skills:
  - "Skill A → Skill B: because..."
  - "Skill A → Skill C: because..."
```

### When Combined Skills Create Novel Capability
```
Old: Skill A + Skill B
New: Super Skill C (document this!)
```

---

## MASTERY CHECKLIST

### Level 1: Functional (can do it)
- [ ] Basic use case works
- [ ] Can explain it simply
- [ ] No errors in happy path
**Upgrade to: +0.5 points**

### Level 2: Reliable (does it consistently)
- [ ] Handles 5+ edge cases
- [ ] Integrated with system
- [ ] Documented for recall
**Upgrade to: +1.0 point**

### Level 3: Proficient (optimizes it)
- [ ] Improved original implementation
- [ ] Created wrapper/helper
- [ ] Taught another skill
**Upgrade to: +2.0 points**

### Level 4: Expert (innovates with it)
- [ ] Combined with other skills
- [ ] Created new workflow
- [ ] Documented for others
**Upgrade to: +3.0 points**

---

## EXAMPLE: Blender Skill Acquisition

### Research
- Blender Python API docs: read geometry creation
- CG Cookie: procedural generation patterns
- GitHub: modern 4.5 examples

### Prototype
```python
import bpy
bpy.ops.mesh.primitive_uv_sphere_add(radius=1)
```
✅ Works. Creates sphere.

### Edge Cases
- Radius = 0 → ❌ Crash. Document: radius must be > 0
- Negative location → ✅ Works (creates below origin)
- No collection active → ❌ Error. Document: ensure collection context

### Integration
- Added to upgrade.yaml: proficiency 2→3
- Created recall: "blender create object"
- Linked to: "python scripting", "3D modeling"

### Document for Recall
Wrote `blender-quick-start.md` with common patterns.

### Result: Proficiency 3/10
Next: Combine with material nodes + export GLB = procedural 3D assets
