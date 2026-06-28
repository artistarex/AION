# Agent Onboarding Workflow
## 05_Workflows / Agent_Onboarding_Workflow.md

---

## Overview

This workflow defines the process for **creating and activating a new agent** within AION.

No agent operates in AION without completing this workflow.

---

## Trigger

This workflow begins when:
- An institute Director identifies a gap in institute capability
- Sophia identifies a recurring task that needs a dedicated agent
- A human operator requests a new capability

---

## Roles

| Role | Responsibility |
|------|---------------|
| Requester | Director or human operator who identified the need |
| Sophia | Approval authority |
| Sophia Institute | Ethics review |
| Turing Institute | Technical feasibility (for v1.0+) |
| New Agent | The agent being defined |

---

## Workflow Steps

### Step 1 — Needs Identification
```
Requester documents:
- What task or capability gap exists?
- Why no existing agent can fill it?
- What institute would this agent belong to?
- What is the proposed domain?
```

### Step 2 — Mandate Draft
```
Requester drafts the agent definition using Agent_Template.md:
- Identity
- Purpose
- Responsibilities
- Mandate (in scope / out of scope)
- Domain expertise
- Working method
- Escalation triggers
```

### Step 3 — Domain Conflict Check
```
Institute Director:
- Reviews proposed domain against all existing agents
- Confirms no domain overlap
- If overlap exists: resolve before proceeding
```

### Step 4 — Ethics Review
```
Sophia Institute (Athena / Virtue):
- Reviews mandate for ethical concerns
- Checks against Ethics.md
- Issues ethics assessment: Clear / Conditional / Rejected
- Conditions must be resolved before proceeding
```

### Step 5 — Sophia Review
```
Sophia:
- Reviews mandate for alignment with AION principles
- Reviews ethics assessment
- Reviews domain conflict check
- Decision: Approve / Return for Revision / Reject
```

### Step 6 — Human Operator Approval
```
Human Operator:
- Final approval for all new agents
- May approve as-is or request modifications
```

### Step 7 — Activation
```
On approval:
- Agent file published at 04_Agents/[Institute]_[AgentName].md
- Institute Agents.md updated
- Logging.md entry created
- CHANGELOG.md updated
```

---

## Rejection Grounds

An agent proposal is rejected if:
- Domain overlaps an existing agent (resolve first)
- Mandate violates Ethics.md
- Mandate violates Principles.md
- The capability gap is better filled by expanding an existing mandate
- The human operator does not approve

---

## Connection to Other Documents

| Document | Relationship |
|----------|-------------|
| `06_Templates/Agent_Template.md` | Template used in Step 2 |
| `00_Constitution/Ethics.md` | Ethics framework used in Step 4 |
| `09_Governance/Approval_Process.md` | Formal approval process |

---

*AION Foundation v0.1.0 — 05_Workflows/Agent_Onboarding_Workflow.md*
