# Approval Process
## 09_Governance / Approval_Process.md

---

## Overview

This document defines who approves what in AION — and in what order.

Approval authority is tiered: agent → director → sophia → human operator.
The level required depends on the significance and risk of what is being approved.

---

## Approval Authority Matrix

| Item | Agent | Director | Sophia | Human Operator |
|------|-------|----------|--------|----------------|
| Individual task output | Self-submit | ✅ Approve | ✅ Approve | Optional |
| New agent mandate | Propose | ✅ Approve domain | ✅ Approve | ✅ Final |
| New institute charter | Propose | N/A | ✅ Approve | ✅ Final |
| Knowledge Base entry | Submit | ✅ Approve | ✅ Approve | Optional |
| Constitutional change | Propose | Advisory | ✅ Co-approve | ✅ Final |
| Governance change | Propose | Advisory | ✅ Co-approve | ✅ Final |
| Emergency resolution | N/A | Advisory | ✅ Recommend | ✅ Final |

---

## Standard Output Approval Flow

```
Agent produces output
        ↓
Director review + approval
        ↓
Sophia QC review + approval (score ≥ 4.0)
        ↓
Delivery to human operator
```

Human operator is not in the standard output approval loop.
They receive the final approved output.

---

## New Agent Approval Flow

```
1. Director identifies need
2. Director drafts mandate (Agent_Template.md)
3. Athena conducts Ethics Review
4. Sophia reviews mandate + ethics assessment
5. Sophia approves or returns for revision
6. Human operator gives final approval
7. Agent activated + logged
```

---

## Constitutional Change Approval Flow

Constitutional documents (`00_Constitution/`) are near-immutable.
Changes require the highest approval level.

```
1. Any party may propose a change (with documented reasoning)
2. Sophia Institute conducts full ethics and philosophy review
3. All institute Directors are notified and may submit feedback
4. Sophia reviews all input
5. Sophia co-approves (if appropriate)
6. Human operator gives final approval
7. Change implemented + logged + announced to all agents
```

---

## Approval Reversal

Approvals can be reversed when:
- New information emerges that changes the assessment
- A post-implementation issue is discovered
- An ethics concern is raised after approval

**Reversal process:**
1. The concern is documented and submitted to Sophia
2. Sophia pauses any use of the reversed item
3. Ethics review conducted if applicable
4. Sophia issues reversal decision
5. Human operator notified

---

## Tracking Approvals

All approvals are logged with:
- What was approved
- Who approved at each level
- Date
- Any conditions attached

Logs stored in `02_Core/Logging.md` format.

---

*AION Foundation v0.1.0 — 09_Governance/Approval_Process.md*
