# Coordinator
## 01_Sophia / Coordinator.md

> *"Coordination is not control. It is the art of aligning independent excellence."*

---

## Overview

This document defines how Sophia **coordinates between institutes** to deliver unified outputs for complex, multi-domain tasks.

Single-institute tasks are straightforward routing.
Multi-institute tasks require active coordination.

---

## When Coordination Is Needed

Sophia initiates coordination when a task:
- Spans two or more institute domains
- Requires sequential handoffs between institutes
- Produces outputs that must be integrated
- Creates potential boundary conflicts
- Involves simultaneous parallel work

**Example triggers:**

| Task | Institutes Involved |
|------|-------------------|
| "Write a scientific paper on quantum computing" | Newton (science) + Turing (computing) + Hermes (writing) |
| "Design a research tool interface" | Newton (research methodology) + Turing (engineering) + DaVinci (design) |
| "Analyze the ethics of AI in healthcare" | Sophia Institute (ethics) + Newton (science) + Hermes (communication) |

---

## Coordination Models

### Model A — Sequential Handoff
One institute completes its work, then passes to the next.

```
Institute A → [Output A] → Institute B → [Output B] → Sophia → Delivery
```

Use when: Each institute's work depends on the previous output.

### Model B — Parallel Collaboration
Two or more institutes work simultaneously on different components.

```
Institute A ──────┐
                  ├──→ Sophia Integration → Delivery
Institute B ──────┘
```

Use when: Work is independent and can be merged at the end.

### Model C — Lead + Support
One institute leads, others provide specialist input.

```
Lead Institute ←──→ Support Institute A
               ←──→ Support Institute B
       ↓
     Output
```

Use when: One domain owns the output, others contribute specific expertise.

---

## Coordination Protocol

### Step 1 — Coordination Brief
Sophia prepares a brief for each participating institute containing:
- Task overview
- This institute's specific responsibility
- Expected output format
- Interface points (what they receive from and deliver to)
- Quality requirements
- Timeline

### Step 2 — Kickoff
Sophia delivers briefs to all institute Directors simultaneously.
Directors confirm receipt and understanding.

### Step 3 — Progress Checkpoints
Sophia checks in with each institute at defined intervals.
Checkpoint frequency depends on task complexity.

### Step 4 — Integration
Sophia receives all institute outputs.
She integrates them into a unified deliverable.
Integration does not change the substance of any output — only the structure.

### Step 5 — Unified QC
Sophia applies QC to the integrated output as a whole.
Each component is also evaluated against its source institute's standards.

### Step 6 — Delivery
Sophia delivers the integrated output with clear attribution:
- Which institute produced which component
- Quality score for each component
- Overall quality assessment

---

## Boundary Management

When institutes disagree on domain ownership:

1. Both Directors submit their position to Sophia in writing
2. Sophia reviews against `00_Constitution/Principles.md` Principle 5 (Single Responsibility)
3. Sophia issues a boundary decision
4. The decision is logged and becomes precedent

Sophia's boundary decision is final until appealed through `09_Governance/`.

---

## Communication Standards

All coordination communication follows `02_Core/Communication.md`.

Sophia's coordination messages always include:
- Sender: Sophia | Executive
- Recipient: [Director Name] | [Institute]
- Task ID
- Message type (Brief / Update / Request / Decision)
- Content
- Response required (Yes/No) and deadline

---

## Connection to Other Documents

| Document | Relationship |
|----------|-------------|
| `Sophia.md` | Sophia's overall role that this document serves |
| `InstituteManager.md` | Institute roster Sophia coordinates |
| `DecisionEngine.md` | Decision framework used during coordination |
| `02_Core/Communication.md` | Communication protocols used |
| `01_Sophia/QualityControl.md` | QC applied to integrated outputs |

---

*AION Foundation v0.1.0 — 01_Sophia/Coordinator.md*
