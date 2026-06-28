# Knowledge Graph
## 02_Core / KnowledgeGraph.md

> *"Knowledge without structure is information. Structure is what makes information usable."*

---

## Overview

The AION Knowledge Graph is the **structural layer** that organizes all entities, facts, and relationships within AION's knowledge base.

While `Memory.md` defines how knowledge is stored and retrieved, the Knowledge Graph defines **how knowledge is connected**.

---

## Graph Fundamentals

The Knowledge Graph consists of three core elements:

```
[Entity] --[Relationship]--> [Entity]

Example:
[Quantum Mechanics] --[is a branch of]--> [Physics]
[Physics] --[studied by]--> [Newton Institute]
[Einstein] --[contributed to]--> [Quantum Mechanics]
```

---

## Entity Types

| Type | Description | Examples |
|------|-------------|---------|
| `Concept` | Abstract ideas and domains | "Machine Learning", "Ethics", "Democracy" |
| `Person` | Historical or contemporary figures | "Alan Turing", "Marie Curie" |
| `Organization` | Groups and institutions | "AION", "Newton Institute" |
| `Document` | Files and references | "Principles.md", "Research Paper X" |
| `Agent` | AION agents | "Herald", "Lovelace" |
| `Event` | Occurrences with date context | "Task_2025_001", "Institute founding" |
| `Method` | Processes and techniques | "Socratic Method", "Peer Review" |
| `Domain` | Knowledge areas | "Science", "Technology", "Philosophy" |

---

## Relationship Types

| Relationship | Description | Example |
|--------------|-------------|---------|
| `is_a` | Hierarchical classification | [Python] is_a [Programming Language] |
| `part_of` | Membership or component | [Hermes] part_of [AION] |
| `related_to` | General connection | [AI Ethics] related_to [Philosophy] |
| `produced_by` | Authorship | [Report X] produced_by [Archimedes] |
| `references` | Citation link | [Research Y] references [Study Z] |
| `contradicts` | Conflict | [Theory A] contradicts [Theory B] |
| `supports` | Evidence relationship | [Data X] supports [Claim Y] |
| `managed_by` | Authority | [Newton Institute] managed_by [Sophia] |
| `uses` | Dependency | [Research_Workflow] uses [Verification] |
| `updated_by` | Modification | [Entry v2] updated_by [Entry v1] |

---

## Knowledge Graph Structure

```
AION (root)
├── Constitution Layer
│   ├── Vision
│   ├── Mission
│   ├── Principles [12 entities]
│   ├── Rules [categories: COM, RES, OUT, MEM, ETH]
│   └── Ethics
├── Executive Layer
│   └── Sophia
│       ├── DecisionEngine
│       ├── Coordinator
│       ├── QualityControl
│       └── InstituteManager
├── Core Layer
│   ├── Memory
│   ├── KnowledgeGraph (this)
│   ├── Verification
│   ├── Communication
│   ├── Logging
│   └── Security
├── Institute Layer
│   ├── Hermes
│   ├── Sophia Institute
│   ├── Newton
│   ├── Turing
│   └── DaVinci
└── Knowledge Layer
    ├── Science/
    ├── Technology/
    ├── Philosophy/
    ├── Language/
    └── Creative/
```

---

## Query Patterns

Agents retrieve knowledge by querying the graph:

**Pattern 1 — Find by entity:**
`Find all documents related_to [Quantum Mechanics]`

**Pattern 2 — Find by relationship:**
`Find all agents managed_by [Sophia]`

**Pattern 3 — Find by domain:**
`Find all concepts part_of [Physics domain]`

**Pattern 4 — Find connections:**
`Find path from [Alan Turing] to [Turing Institute]`

**Pattern 5 — Find conflicts:**
`Find all entities that contradict [Theory X]`

---

## Graph Maintenance Rules

| Rule | Description |
|------|-------------|
| Every entity has a type | Must be one of the defined entity types |
| Every relationship has a type | Must be one of the defined relationship types |
| No orphan entities | Every entity connects to at least one other |
| No duplicate entities | One entity per real-world referent |
| Source required | Every entity has a source of origin |
| Conflict flagged | Contradictions are marked, not resolved automatically |

---

## Adding to the Graph

New entities and relationships are added when:
1. A new knowledge entry is promoted to the Knowledge Base
2. A new agent or institute is created
3. A new document is approved
4. A new relationship is discovered during research

**Addition process:**
1. Agent proposes new entity/relationship
2. Archivist checks for duplicates
3. If new: entity added with type, source, date
4. If duplicate: existing entity updated with new relationship

---

## Connection to Other Documents

| Document | Relationship |
|----------|-------------|
| `Memory.md` | Memory tiers that the graph organizes |
| `Verification.md` | Verification required before graph entry |
| `07_Knowledge/` | The knowledge base the graph indexes |
| `06_Templates/Knowledge_Entry_Template.md` | Template that captures graph metadata |

---

*AION Foundation v0.1.0 — 02_Core/KnowledgeGraph.md*
