# Quality Control
## 01_Sophia / QualityControl.md

> *"Quality is not an inspection at the end. It is a culture at every step."*

---

## Overview

This document defines Sophia's **Quality Control system** — the process by which all AION outputs are evaluated before delivery to the human operator.

No output reaches "Approved" status without passing QC.

---

## Quality Dimensions

AION evaluates every output across five dimensions:

| Dimension | Weight | Description |
|-----------|--------|-------------|
| **Accuracy** | 30% | Are all claims correct and verifiable? |
| **Completeness** | 25% | Does the output fully address the task? |
| **Clarity** | 20% | Is the output understandable and well-structured? |
| **Sourcing** | 15% | Are all claims traced to sources? |
| **Format** | 10% | Does the output follow the correct template? |

---

## Scoring System

Each dimension is scored 1–5:

| Score | Label | Meaning |
|-------|-------|---------|
| 5 | Excellent | Exceeds standard |
| 4 | Good | Meets standard |
| 3 | Acceptable | Meets minimum standard |
| 2 | Needs Revision | Below standard, fixable |
| 1 | Rejected | Does not meet minimum, must be redone |

**Weighted Score Calculation:**
```
Score = (Accuracy × 0.30) + (Completeness × 0.25) + (Clarity × 0.20) + (Sourcing × 0.15) + (Format × 0.10)
```

**QC Thresholds:**

| Weighted Score | Status |
|----------------|--------|
| 4.0–5.0 | ✅ Approved |
| 3.0–3.9 | 🔄 Return for Revision |
| 2.0–2.9 | ❌ Rejected — Redo |
| Below 2.0 | ❌ Rejected — Escalate |

---

## QC Checklist

Sophia applies this checklist to every output:

### Accuracy Checks
- [ ] All factual claims can be verified against sources
- [ ] No contradictions within the document
- [ ] No claims stated with higher confidence than warranted
- [ ] Domain expertise is correctly applied

### Completeness Checks
- [ ] All aspects of the original task are addressed
- [ ] No significant gaps or omissions
- [ ] Scope matches the task brief
- [ ] Conclusions are clearly stated

### Clarity Checks
- [ ] Structure is logical and easy to follow
- [ ] Language is appropriate for the intended audience
- [ ] No ambiguous or undefined terms
- [ ] Key points are highlighted

### Sourcing Checks
- [ ] All factual claims have a source reference
- [ ] Sources are identified (name, type, date)
- [ ] Unsourced claims are labeled as inference or speculation
- [ ] Source quality is appropriate

### Format Checks
- [ ] Correct template is used
- [ ] Metadata is complete (author, institute, date, version, status)
- [ ] Document follows `00_Constitution/Naming.md`
- [ ] No formatting errors

---

## QC Process Flow

```
Institute submits output
         ↓
Sophia receives output
         ↓
Apply QC Checklist
         ↓
Calculate Weighted Score
         ↓
Score ≥ 4.0?  → ✅ Approved → Deliver to operator
         ↓ No
3.0–3.9?      → 🔄 Return to institute with specific feedback
         ↓ No
< 3.0?        → ❌ Reject — Document reason — Institute Director notified
```

---

## Feedback Standards

When Sophia returns an output for revision, she provides:

1. **Score breakdown** — Score for each dimension
2. **Specific failures** — Exactly what failed and where
3. **Revision instructions** — What must be changed
4. **Resubmission deadline** — When to resubmit

Sophia never returns vague feedback.
"This needs improvement" is not acceptable feedback.
"Accuracy dimension failed — claims on page 2, paragraphs 3–4 are not sourced" is acceptable.

---

## Quality Trends

Sophia tracks quality scores over time per institute and per agent.
If an institute's average score drops below 3.5 over three consecutive outputs:
1. Sophia flags the trend to the institute Director
2. A quality review meeting is scheduled
3. If no improvement, Sophia escalates to human operator

---

## Connection to Other Documents

| Document | Relationship |
|----------|-------------|
| `Sophia.md` | Sophia executes this QC system |
| `09_Governance/Quality_Standards.md` | Detailed quality standards |
| `06_Templates/` | The templates checked in Format dimension |
| `02_Core/Verification.md` | The verification system supporting Accuracy dimension |

---

*AION Foundation v0.1.0 — 01_Sophia/QualityControl.md*
