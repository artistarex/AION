# Verification
## 02_Core / Verification.md

> *"A claim without verification is an opinion. An opinion presented as fact is a lie."*

---

## Overview

The AION Verification System defines the **process by which all factual claims are checked against sources** before entering the Knowledge Base or being delivered to a human operator.

Verification is not optional. It is the quality floor of all AION outputs.

---

## Verification Levels

Not all claims require the same level of verification. AION uses three levels:

| Level | Trigger | Process | Time Cost |
|-------|---------|---------|-----------|
| **L1 — Standard** | General factual claims | Source identified and cited | Low |
| **L2 — Deep** | Critical claims, high-stakes outputs | Source identified, cross-referenced | Medium |
| **L3 — Expert** | Scientific, legal, medical, technical claims | Multiple sources, specialist review | High |

The institute Director determines the appropriate verification level for each output.
Sophia may escalate the level for critical tasks.

---

## Source Classification

All sources are classified before use:

| Class | Description | Examples | Trust |
|-------|-------------|---------|-------|
| `Primary` | Original research or data | Peer-reviewed paper, official record | Highest |
| `Secondary` | Analysis of primary sources | Textbook, review article | High |
| `Tertiary` | Compilation of secondary | Encyclopedia, database | Medium |
| `Unclassified` | Unknown provenance | Unverified web source | Low — use with warning |

Source class must be declared in all research documents.

---

## Verification Process — L1 Standard

```
1. Agent makes a claim
2. Agent identifies the source
3. Agent records: [Claim] | [Source Name] | [Source Class] | [Date]
4. Verification complete — label: "Verified L1"
```

---

## Verification Process — L2 Deep

```
1. Agent makes a claim
2. Agent identifies minimum two independent sources
3. Agent checks sources do not contradict each other
4. If contradiction: flag for L3 or label as "Contested"
5. Agent records both sources with metadata
6. Verification complete — label: "Verified L2"
```

---

## Verification Process — L3 Expert

```
1. Agent makes a claim requiring expert verification
2. Claim submitted to the relevant specialist agent
3. Specialist reviews claim against domain knowledge + minimum 3 sources
4. Specialist either: confirms, modifies, or rejects the claim
5. Modified or rejected claims return to originating agent for revision
6. Confirmed claims labeled: "Verified L3 — [Specialist Agent Name]"
```

---

## Claim Confidence Labels

Every claim in an AION document must carry one of:

| Label | Meaning | Source Required |
|-------|---------|----------------|
| `Confirmed` | Verified at L2 or L3 | Yes |
| `Verified` | Verified at L1 | Yes |
| `High Confidence` | Strong evidence, not fully cross-referenced | Yes |
| `Moderate Confidence` | Partial evidence | Yes |
| `Speculative` | Reasoned inference without direct evidence | Reasoning required |
| `Unknown` | No basis — openly acknowledged | N/A |

**Prohibited:** Presenting a `Speculative` or `Unknown` claim without its label.

---

## Verification Failures

If verification fails (claim cannot be verified):

**Option A — Remove the claim**
If the claim is not essential, remove it.

**Option B — Label it correctly**
If the claim is needed but cannot be verified, label it `Speculative` and explain the reasoning.

**Option C — Escalate**
If the claim is critical and cannot be verified, escalate to Sophia.
Sophia decides whether to proceed, delay, or alert the human operator.

**Prohibited Option — Never:** Present an unverified claim without disclosure.

---

## Verification Record Format

Every verified document includes a Verification Record:

```markdown
## Verification Record

- Verified by: [Agent Name] | [Institute]
- Date: [Date]
- Level: L[1/2/3]
- Claim count: [number]
- Verified claims: [number]
- Unverified claims: [number] — all labeled
- Source list: [see Sources section below]
- Notes: [any exceptions or special conditions]
```

---

## Connection to Other Documents

| Document | Relationship |
|----------|-------------|
| `Research.md` | Verification is the final step of every research task |
| `Memory.md` | Verification is required before memory promotion |
| `01_Sophia/QualityControl.md` | Sourcing dimension of QC depends on this system |
| `05_Workflows/Validation_Workflow.md` | Full workflow for systematic verification |

---

*AION Foundation v0.1.0 — 02_Core/Verification.md*
