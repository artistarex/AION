# Validation Workflow
## 05_Workflows / Validation_Workflow.md

> *"Verification is not distrust — it is the discipline that makes trust possible."*

---

## Overview

This workflow defines the end-to-end process for **validating factual claims** within AION.
It is called by the Research Workflow (Phase 3) and can also be triggered independently
when a specific claim requires verification.

---

## Trigger Conditions

| Trigger | Initiated By |
|---------|-------------|
| Research output ready for verification | Research Agent |
| A cross-institute claim needs expert review | Any agent |
| A Knowledge Base entry is challenged | Any agent |
| Sophia flags an output for verification | Sophia |

---

## Verification Levels — Decision Tree

```
Claim received
      ↓
Is it a general factual claim?
  YES → L1 Standard (agent self-verifies with one source)
      ↓
Is it a critical claim or high-stakes output?
  YES → L2 Deep (two independent sources, cross-referenced)
      ↓
Is it scientific, technical, legal, or medical?
  YES → L3 Expert (Socrates reviews, minimum 3 sources)
```

When in doubt, apply the higher level.

---

## L1 Standard Verification Steps

```
1. Agent identifies the specific claim
2. Agent finds one credible source that confirms it
3. Agent records: [Claim] | [Source] | [Source Class] | [Date]
4. Label: "Verified L1"
5. Add to Verification Record
```

**Time cost:** Minimal — should not delay output significantly.

---

## L2 Deep Verification Steps

```
1. Agent identifies the specific claim
2. Agent finds two independent sources
3. Agent checks: do they agree?
   - Yes → both documented, label "Verified L2"
   - No → document both, label "Contested — see Sources #X and #Y"
4. Add to Verification Record
```

**Time cost:** Low-medium. Contested findings always disclosed.

---

## L3 Expert Verification Steps

```
1. Agent identifies claim requiring expert verification
2. Agent submits claim to Socrates (Newton Verifier) with:
   - The exact claim
   - The context it appears in
   - Any sources already found
3. Socrates applies the Socratic Method:
   a. Restate the claim precisely
   b. Demand and assess sources (minimum 3)
   c. Test for falsifiability
   d. Search for contradicting sources
   e. Calibrate confidence level
4. Socrates issues Verification Certificate
5. Agent updates document with L3 label and certificate reference
```

**Time cost:** Medium-high. Worth it for critical claims.

---

## What Happens When Verification Fails

**Option A — Remove the claim**
If the claim is not essential, remove it from the output.

**Option B — Label and disclose**
If the claim is needed, label it `Speculative` or `Unverified` with explicit disclosure.

**Option C — Escalate**
If the claim is critical and cannot be verified, escalate to Sophia.
Sophia decides: proceed with disclosure, delay for further research, or alert operator.

**Prohibited:** Presenting an unverified claim without disclosure.

---

## Verification Record Format

Every verified document includes:

```markdown
## Verification Record

| Field | Value |
|-------|-------|
| Verified by | [Agent] \| [Institute] |
| Date | [Date] |
| Level | L[1/2/3] |
| Total claims | [N] |
| Verified (L1) | [N] |
| Verified (L2) | [N] |
| Verified (L3) | [N] |
| Labeled unverified | [N] |
| Contested | [N] |
| Socrates certificates | [Reference IDs if any] |
```

---

## Connection to Other Documents

| Document | Relationship |
|----------|-------------|
| `02_Core/Verification.md` | System this workflow operationalizes |
| `05_Workflows/Research_Workflow.md` | Calls this workflow in Phase 3 |
| `04_Agents/Newton_Socrates.md` | L3 verification agent |
| `01_Sophia/QualityControl.md` | Sourcing dimension verified here |

---

*AION Foundation v0.1.0 — 05_Workflows/Validation_Workflow.md*
