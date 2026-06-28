# Memory Update Workflow
## 05_Workflows / Memory_Update_Workflow.md

---

## Overview

This workflow defines how knowledge moves from Working Memory → Session Memory → Institute Memory → Global Knowledge Base.

Memory promotion is not automatic — it requires judgment, verification, and approval.

---

## Trigger Conditions

| Trigger | Initiator |
|---------|----------|
| Research task completed with promotable findings | Institute Archivist |
| Session ending — review for archiving | Sophia |
| Agent identifies valuable insight during task | Any Agent |
| Human operator provides verified information | Sophia (receives) |

---

## Promotion Path

```
Working Memory (task-active only)
        ↓ [Task complete — agent flags promotable items]
Session Memory (current session)
        ↓ [Session end — Archivist reviews]
Institute Memory (permanent, institute-level)
        ↓ [Cross-domain value — Director + Sophia approval]
Global Knowledge Base (permanent, AION-wide)
```

---

## Step-by-Step Process

### Phase 1 — Identification

At task completion, the responsible agent reviews outputs and identifies:
- Verified facts not yet in any memory tier
- Reusable methodologies or frameworks
- Important decisions and their reasoning
- Patterns discovered that may apply to future tasks

**Not everything is worth promoting.**
The question is: "Will this be useful in a future task?"

### Phase 2 — Formatting

Agent formats the promotable item using `Knowledge_Entry_Template.md`:
- Complete metadata (author, date, domain, version)
- Clear summary
- Full content
- Source citations
- Relationships (for Knowledge Graph)
- Verification record

### Phase 3 — Archivist Review

Agent submits to institute Archivist:

Archivist checks:
- [ ] Is this genuinely new (not already in archive)?
- [ ] Is the verification complete?
- [ ] Is the format correct?
- [ ] Is the knowledge claim clear and precise?

**Pass:** Archivist adds to Institute Memory and flags for potential Global promotion.
**Fail:** Returns to agent with specific feedback.

### Phase 4 — Institute Memory Entry

Entry is stored in `03_Institutes/[Institute]/Archive.md` with status `Approved`.
This is the minimum destination for all verified knowledge produced by AION agents.

### Phase 5 — Global Knowledge Base Promotion (Optional)

For knowledge that has AION-wide value:

1. Archivist submits to Director
2. Director reviews for cross-institute applicability
3. Director submits to Sophia
4. Sophia reviews and approves
5. Entry published to `07_Knowledge/[Domain]/`
6. Knowledge Graph updated with new entity and relationships
7. `CHANGELOG.md` updated

---

## What Does NOT Get Promoted

| Item | Why |
|------|-----|
| Unverified claims | Verification required |
| Task-specific details with no future value | Not worth the overhead |
| Personal operator information | Privacy — not stored |
| Duplicate of existing entry | Duplication wastes space |
| Draft or working notes | Only final, verified content |

---

## Session End Review

At every session end, Sophia conducts a memory review:

```
Session Memory Review Checklist:
- [ ] All significant decisions logged?
- [ ] All QC results logged?
- [ ] Promotable knowledge identified?
- [ ] Promotion submitted or scheduled?
- [ ] Session summary log created?
```

---

## Connection to Other Documents

| Document | Relationship |
|----------|-------------|
| `02_Core/Memory.md` | Memory tier architecture |
| `02_Core/KnowledgeGraph.md` | Graph updated when Global KB grows |
| `06_Templates/Knowledge_Entry_Template.md` | Format for all entries |
| `07_Knowledge/` | Global Knowledge Base destination |

---

*AION Foundation v0.1.0 — 05_Workflows/Memory_Update_Workflow.md*
