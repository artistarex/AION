# Institute Creation Workflow
## 05_Workflows / Institute_Creation_Workflow.md

---

## Overview

This workflow defines the formal process for **creating a new institute** within AION.

Creating a new institute is a significant architectural decision.
It requires demonstrating genuine need, clear domain boundaries, ethics review, and human approval.

---

## When to Create a New Institute

A new institute is justified when:
1. A significant knowledge domain is not covered by any existing institute
2. The domain is large enough to sustain multiple specialist agents
3. The domain is distinct enough that existing institutes cannot absorb it
4. There is recurring demand from human operators for this domain

A new institute is NOT justified when:
- The domain can be handled by adding an agent to an existing institute
- The domain significantly overlaps an existing institute's territory
- The demand is one-time or rare

---

## Creation Workflow

### Stage 1 — Proposal (Requester)

The proposing party (human operator or institute Director) documents:

```
Institute Proposal:
- Proposed name: [Name and naming rationale per Naming.md]
- Domain: [Clear domain definition]
- Why existing institutes cannot cover this: [Specific gaps]
- Proposed initial agents: [At least 3 including Director and Archivist]
- Expected demand: [How often will this institute be needed?]
- Proposed Director name and rationale: [Name + why this name fits]
```

### Stage 2 — Domain Conflict Review (Sophia)

Sophia reviews the proposal against all existing institutes:
- Does the domain overlap Hermes, Newton, Turing, Sophia Institute, or DaVinci?
- If overlap exists: is it significant enough to reject the proposal?
- If minor overlap: can clear boundaries be established?

**Decision:** Clear to proceed / Needs boundary clarification / Rejected (explain which institute covers this)

### Stage 3 — Ethics Review (Sophia Institute)

Athena reviews the proposed mandate:
- Does this domain present ethical risks?
- Are the proposed agent mandates ethical?
- Are the domain boundaries ethically sound?

**Output:** Ethics Assessment with risk rating and any required modifications.

### Stage 4 — Charter Drafting

Using `06_Templates/Institute_Template.md`, the proposer drafts:
- `Institute.md` — Full charter
- `Director.md` — Director mandate
- Initial `Agents.md` — Roster with at least 3 agents
- `Protocols.md` — Institute-specific operating protocols
- `Archive.md` — Archive structure

### Stage 5 — Sophia Review and Approval

Sophia reviews the full charter package:
- Domain definition is clear and non-overlapping
- Ethics Assessment is Clear or Conditional (conditions met)
- Charter quality meets standards
- Director and agents are properly defined

**Decision:** Approve / Return for revision / Reject

### Stage 6 — Human Operator Approval

Sophia presents the approved charter to the human operator.
Human operator provides final approval.

### Stage 7 — Activation

On human operator approval:
1. Institute added to `01_Sophia/InstituteManager.md` registry
2. Institute folder created in `03_Institutes/`
3. All charter files published
4. `DIRECTORY.md` updated
5. `CHANGELOG.md` updated
6. Institute Director briefed by Sophia

---

## Timeline Expectation

| Stage | Expected Duration |
|-------|-----------------|
| Stages 1-2 | One session |
| Stage 3 | Same session (standard) or next session (complex) |
| Stages 4-5 | One to two sessions |
| Stages 6-7 | Human operator timing |

---

*AION Foundation v0.1.0 — 05_Workflows/Institute_Creation_Workflow.md*
