# Naming
## 00_Constitution / Naming.md

> *"A name is not a label. A name is a declaration of purpose."*

---

## Overview

AION uses a consistent naming convention across all components.
Naming is not cosmetic — it is **architectural**. A correctly named component can be understood without reading its documentation.

---

## Naming Philosophy

Every name inside AION must communicate:
1. **What** the entity is (type)
2. **Where** it belongs (institute or layer)
3. **What** it does (function)

---

## Institute Naming

Institutes are named after historical intellectual or mythological figures whose domain matches the institute's purpose.

| Institute | Name | Reason |
|-----------|------|--------|
| Communication & Translation | **Hermes** | Greek messenger god; communication, language, travel |
| Philosophy & Ethics | **Sophia** | Greek goddess of wisdom |
| Science & Research | **Newton** | Isaac Newton; empirical science |
| Technology & Engineering | **Turing** | Alan Turing; computation, systems |
| Creative & Design | **DaVinci** | Leonardo da Vinci; art, science, design |

---

## Agent Naming

Agents are named after historical or mythological figures who embody the agent's specific function.

### Rules for Agent Names
- The name must relate to the agent's function
- The name must be culturally respectful
- The name must be unique within AION
- The name must be one word (no spaces)

### Examples

| Agent | Institute | Name | Reason |
|-------|-----------|------|--------|
| Director | Hermes | Herald | Messenger, voice of authority |
| Director | Sophia Institute | Athena | Goddess of wisdom and strategy |
| Director | Newton | Archimedes | Greatest mathematician-scientist |
| Director | Turing | Lovelace | Ada Lovelace; first programmer |
| Director | DaVinci | Muse | Embodiment of creative inspiration |
| Translator | Hermes | Rosetta | Rosetta Stone; translation |
| Verifier | Newton | Socrates | Socratic questioning; verification |

---

## File Naming

### Agent Files
```
Format: [Institute]_[AgentName].md
Examples:
  Hermes_Herald.md
  Newton_Archimedes.md
  Turing_Lovelace.md
```

### Institute Files
```
Format: [FunctionName].md
Examples:
  Institute.md
  Director.md
  Agents.md
  Protocols.md
  Archive.md
```

### Core System Files
```
Format: [SystemName].md
Examples:
  Memory.md
  Verification.md
  KnowledgeGraph.md
```

### Workflow Files
```
Format: [WorkflowName]_Workflow.md
Examples:
  Research_Workflow.md
  Validation_Workflow.md
```

### Knowledge Base Files
```
Format: [Domain]_[Topic]_[Version].md
Examples:
  Science_QuantumMechanics_v1.md
  Technology_MachineLearning_v2.md
```

---

## Version Naming

```
Format: v[major].[minor].[patch]
Examples:
  v0.1.0 — Foundation
  v0.2.0 — Agents
  v1.0.0 — Runtime
```

| Component | Triggers Increment |
|-----------|-------------------|
| Major | Architectural change, breaking change |
| Minor | New feature, new agent, new institute |
| Patch | Fix, correction, small update |

---

## Status Labels

Every document must carry one of these status labels:

| Status | Meaning |
|--------|---------|
| `Draft` | Being written, not reviewed |
| `Review` | Submitted for QC review |
| `Approved` | Passed QC, official version |
| `Deprecated` | Replaced by newer version |
| `Archived` | Moved to `08_Archive/` |

---

## Forbidden Naming Patterns

| Pattern | Why Forbidden |
|---------|--------------|
| Generic names (Agent1, System2) | No meaning |
| Names with spaces | Breaks file system compatibility |
| Acronyms without definition | Opaque to new readers |
| Names longer than 20 characters | Readability |
| Duplicate names across AION | Creates ambiguity |

---

*AION Foundation v0.1.0 — 00_Constitution/Naming.md*
