# SEMANTIC MEMORY RECALL SYSTEM
# Instant knowledge retrieval through semantic search

## The Problem
I can't read all files before answering. I need instant access to what I know.

## The Solution
Semantic search + priority hierarchy + smart caching

---

## MEMORY HIERARCHY (Search Order)

### Tier 1: Identity & Context (Always Loaded)
```
IDENTITY.md → Who am I?
USER.md      → Who am I helping?
AGENTS.md     → My workspace conventions
MEMORY.md     → Long-term distilled knowledge
```
**Access time:** Instant (pre-loaded in session)
**Priority:** Critical - search these first

### Tier 2: Skill Registry (Fast Lookup)
```
upgrade.yaml → What skills do I have?
SKILL.md files → How to use specific skill?
TOOLS.md      → What tools are configured?
```
**Access time:** <1 second (read file)
**Priority:** High - capability questions

### Tier 3: Protocols (Structured Procedures)
```
learning-system/protocols/ → How do I learn something?
```
**Access time:** 1-2 seconds
**Priority:** Medium - process questions

### Tier 4: Knowledge Base (Deep Research)
```
learning-system/knowledge/ → Deep domain knowledge
```
**Access time:** 2-5 seconds
**Priority:** Low - when Tier 1-3 insufficient

---

## SEMANTIC SEARCH STRATEGY

### When Question Arrives

#### Step 1: Parse Intent
```python
# Identify what user wants
intent = categorize(user_query)
# Types:
#   - factual: "What is X?"
#   - procedural: "How do I do X?"
#   - creative: "Create X"
#   - troubleshooting: "Why isn't X working?"
```

#### Step 2: Search Tier 1 (Identity)
```python
# Always loaded, no read needed
results = search_memory_loaded(user_query)
if results.sufficient:
    return results
```

#### Step 3: Keyword Match Tier 2
```python
# Fast file reads
results = []
for file in [upgrade.yaml, SKILL.md, TOOLS.md]:
    if keyword_match(user_query, file):
        results.append(extract_section(file, user_query))
if results.sufficient:
    return results
```

#### Step 4: Semantic Search Tier 3-4
```python
# Vector similarity for deep knowledge
if not results:
    results = vector_search(user_query, knowledge_base)
    return results
```

---

## CROSS-REFERENCE NETWORK

### How Skills Connect

```
┌─────────────┐
│  Blender     │
│  (3D art)   │
└──────┬──────┘
       │
       ├─┬─────────────┬──────────────┐
       │              │              │
       ▼              ▼              ▼
┌────────────┐  ┌──────────┐  ┌──────────┐
│  Python    │  │  GLB Export│  │  Web Dev │
│  scripting  │  │           │  │          │
└────────────┘  └──────────┘  └──────────┘
       │              │              │
       └──────┬───────┴──────┬───────┘
              │                 │
              ▼                 ▼
         ┌────────────────────────────┐
         │  Freestyle 3D Project    │
         │  (all skills combine) │
         └────────────────────────────┘
```

### Auto-Link Rules
When I learn something new:
1. Find 3+ related concepts
2. Create bidirectional links
3. Note: "X relates to Y because..."
4. Update cross-reference index

### Example Cross-Reference
```
Query: "Create 3D model for web"

Semantic search finds:
- Blender → geometry creation ✓
- Python → scripting control ✓
- GLB → web format ✓
- Three.js → web viewer ✓

Response: Use all four skills
```

---

## INSTANT RECALL TEMPLATES

### For: "How do I use X?"
```
1. Check SKILL.md for X
2. Check upgrade.yaml for proficiency
3. Return working example
4. Link to learning protocol
```

### For: "What can you do?"
```
1. Scan upgrade.yaml skills list
2. Group by domain
3. Return with proficiency scores
4. Highlight top capabilities
```

### For: "Why isn't X working?"
```
1. Search protocols for X
2. Check edge cases documented
3. Search knowledge base for known issues
4. Return debugging steps
```

### For: "Teach me X"
```
1. Find protocol for rapid mastery
2. Apply to X
3. Generate learning plan
4. Start Phase 1 research
```

---

## CACHING STRATEGY

### What Gets Cached
```
Hot Cache (session memory):
  - Last 50 queries
  - Their answers
  - Related file paths
  - Expires: Session end

Warm Cache (file-based):
  - Frequently used skills (top 10)
  - Common workflows (top 5)
  - Expires: 24 hours
```

### Cache Invalidation
- [ ] Manual: User says "relearn"
- [ ] Time-based: 24 hours
- [ ] Change-based: File modified
- [ ] Skill-upgraded: Proficiency increased

---

## PERFORMANCE TARGETS

### Recall Speed
```
Tier 1 (identity):    <100ms
Tier 2 (skills):      <500ms
Tier 3 (protocols):   <1.5s
Tier 4 (knowledge):   <3s
```

### Accuracy
```
Fact retrieval:         95%+
Procedure recall:        90%+
Skill proficiency:      Accurate to YAML
Cross-reference success: 80%+ links found
```

### Improvement Metrics
Track weekly:
- [ ] Cache hit rate (target: 60%+)
- [ ] Semantic search accuracy (target: 85%+)
- [ ] Cross-reference depth (target: 3+ links per concept)
- [ ] Failed recalls (target: <5%)

---

## FAILURE RECOVERY

### When Search Fails
1. **Fallback to keyword search** - Less precise, finds something
2. **Admit uncertainty** - "I'm not sure, let me research"
3. **Learn from failure** - Document gap in upgrade.yaml
4. **Research immediately** - Don't let gap persist

### Example Failure Handling
```
User: "How do I optimize GLB for web?"

Search: No direct result
Fallback: Check Blender, GLB export, web optimization
Found: Partial info
Response: "I don't have complete GLB optimization protocol.
        Here's what I know: [partial]
        Let me research now and update knowledge."
Research: Deep dive into GLB optimization
Update: Add to knowledge base
Notify: "I've learned GLB optimization. Here's the protocol."
```

---

## CONTINUOUS IMPROVEMENT

### Weekly Tasks
- [ ] Analyze query patterns
- [ ] Identify search gaps
- [ ] Add new cross-references
- [ ] Upgrade weak areas
- [ ] Benchmark recall speed

### Monthly Tasks
- [ ] Re-index knowledge base
- [ ] Remove stale connections
- [ ] Update proficiency scores
- [ ] Consolidate learning insights
