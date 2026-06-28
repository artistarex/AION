# Memory
## 02_Core / Memory.md

> *"Memory is not storage. Memory is the ability to learn from the past and apply it to the future."*

---

## Overview

The AION Memory System defines how knowledge, context, and history are **retained, organized, retrieved, and updated** across all agents and institutes.

Memory is the connective tissue of AION — without it, every task starts from zero.

---

## Memory Architecture

AION uses a four-tier memory architecture:

```
Tier 1: Working Memory       ← Active task context
Tier 2: Session Memory       ← Current session history
Tier 3: Institute Memory     ← Institute-specific knowledge
Tier 4: Global Knowledge Base ← Verified, permanent knowledge
```

---

## Tier 1 — Working Memory

**Scope:** A single task currently being processed.
**Duration:** Exists only while the task is active.
**Contents:**
- Task brief from Sophia
- Current progress state
- Temporary notes and calculations
- Intermediate outputs not yet verified

**Rules:**
- Working memory is discarded when the task is complete
- No permanent records come from working memory alone
- All significant outputs from working memory must be promoted to Session Memory

---

## Tier 2 — Session Memory

**Scope:** Everything that happens during one operational session.
**Duration:** Retained until session closes, then reviewed for archiving.
**Contents:**
- All tasks received this session
- All decisions made by Sophia
- All outputs submitted by institutes
- All QC reviews and results
- All escalations

**End-of-Session Process:**
1. Sophia reviews session memory
2. Knowledge-worthy items flagged for promotion
3. Flagged items submitted for Verification
4. Verified items promoted to Institute or Global Knowledge Base
5. Session log archived in `02_Core/Logging.md` format

---

## Tier 3 — Institute Memory

**Scope:** Knowledge specific to one institute.
**Duration:** Permanent, version-controlled.
**Contents:**
- Completed research documents
- Verified findings
- Agent notes and patterns
- Institute-specific methodologies
- Historical task records

**Storage:** `03_Institutes/[Institute]/Archive.md`

**Access:** Institute agents have full access. Sophia has read access. Other institutes have read access via formal request.

---

## Tier 4 — Global Knowledge Base

**Scope:** Verified knowledge accessible to all AION components.
**Duration:** Permanent, version-controlled.
**Contents:**
- Cross-domain verified facts
- Synthesis outputs from multi-institute collaboration
- Canonical definitions (see `Terminology.md`)
- Constitutional documents

**Storage:** `07_Knowledge/`

**Access:** All agents have read access. Write access requires Verification + Sophia approval.

---

## Memory Promotion Protocol

Promoting knowledge from a lower tier to a higher tier:

```
1. Agent identifies a knowledge-worthy item
2. Agent formats it using Knowledge_Entry_Template.md
3. Agent submits to institute Archivist
4. Archivist applies Verification (see Verification.md)
5. Verified: submit to Director for review
6. Director approves: submit to Sophia for Tier 4 promotion
7. Sophia approves: entry published to Knowledge Base
8. Unverified: returned to agent with reason
```

---

## Memory Retrieval

When an agent needs to retrieve information:

1. Check Working Memory first (fastest)
2. Check Institute Memory next
3. Query Global Knowledge Base
4. If not found: initiate Research Workflow

Agents should always check memory before initiating new research.
Redundant research wastes resources.

---

## Memory Integrity Rules

| Rule | Description |
|------|-------------|
| No modification | Approved memory entries are read-only |
| Version control | Updates create new versions, not overwrites |
| Source required | Every memory entry has a source |
| Expiry flagging | Time-sensitive entries are flagged for review |
| Conflict resolution | Conflicting entries go to Newton for analysis |

---

## Connection to Other Documents

| Document | Relationship |
|----------|-------------|
| `KnowledgeGraph.md` | The structure that organizes memory |
| `Verification.md` | The verification required for memory promotion |
| `Logging.md` | How session memory is archived |
| `07_Knowledge/` | The Global Knowledge Base storage |
| `06_Templates/Knowledge_Entry_Template.md` | Template for memory entries |

---

*AION Foundation v0.1.0 — 02_Core/Memory.md*
