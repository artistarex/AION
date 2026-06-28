# Research Workflow
## 05_Workflows / Research_Workflow.md

> *"A workflow is a promise — this is exactly how we do this work."*

---

## Overview

This workflow defines the **end-to-end process for all research tasks** within AION.
Every research output, regardless of institute, follows this workflow.

---

## Trigger

This workflow begins when Sophia routes a research task to an institute Director.

---

## Roles

| Role | Responsibility in this Workflow |
|------|--------------------------------|
| Sophia | Task routing, QC, final approval |
| Institute Director | Task assignment, Director review |
| Research Agent | Primary research execution |
| Verifier Agent | Verification (Newton Verifier preferred) |
| Archivist | Knowledge archiving if promoted |
| Hermes (if needed) | Report writing if output is for human delivery |

---

## Workflow Steps

### Phase 1 — Initiation

**Step 1.1 — Task Receipt**
```
Sophia → Director
- Task brief delivered via Communication Layer
- Brief includes: question, expected output, QC requirements, deadline
- Director acknowledges receipt
```

**Step 1.2 — Task Assignment**
```
Director → Research Agent
- Director reviews brief
- Assigns to appropriate research agent
- Director may add institute-specific instructions
- Agent acknowledges assignment
```

**Step 1.3 — Research Statement**
```
Research Agent:
- Reformulates task as a clear Research Statement
- Includes: Primary Question, Sub-questions, Out of Scope, Expected Output
- Submits Research Statement to Director for approval
- Director approves before research begins
```
*Using: Research_Template.md — Research Statement section*

---

### Phase 2 — Research Execution

**Step 2.1 — Source Identification**
```
Research Agent:
- Identifies all potentially relevant sources
- Classifies each source (Primary / Secondary / Tertiary)
- Documents source list
```

**Step 2.2 — Investigation**
```
Research Agent:
- Systematically investigates each source
- Builds findings matrix
- Notes all contradictions
- Does not select only confirming evidence
```

**Step 2.3 — Synthesis**
```
Research Agent:
- Organizes findings by sub-question
- Identifies patterns
- Documents contradictions as contested
- Drafts answers to all research questions
- Identifies limitations
```

---

### Phase 3 — Verification

**Step 3.1 — Self-Verification**
```
Research Agent:
- Labels every claim with confidence level
- Maps every verified claim to its source
- Calculates verification rate
- Completes Verification Record
```

**Step 3.2 — Expert Verification (if L3 required)**
```
Research Agent → Newton Verifier (Socrates):
- Submits claims requiring expert verification
- Socrates reviews against domain knowledge + 3 sources
- Socrates issues verification certificate
- Agent updates document with L3 verification labels
```

---

### Phase 4 — Documentation

**Step 4.1 — Final Document**
```
Research Agent:
- Formats complete output using Research_Template.md
- All metadata complete
- All sections complete
- Verification Record complete
- Status set to "Review"
```

**Step 4.2 — Director Review**
```
Research Agent → Director:
- Submits document for Director Review
- Director applies institute-specific quality standards
- Director returns for revision OR approves for Sophia QC
```

---

### Phase 5 — Quality Control

**Step 5.1 — Sophia QC**
```
Director → Sophia:
- Director submits approved document for Sophia QC
- Sophia applies QualityControl.md checklist
- Sophia scores on 5 dimensions
- Decision: Approve / Return for Revision / Reject
```

**Step 5.2 — Revision (if required)**
```
Sophia → Director → Research Agent:
- Sophia returns specific feedback
- Agent makes required revisions
- Returns to Step 4.2
- Maximum 2 revision cycles before escalation
```

---

### Phase 6 — Delivery and Archiving

**Step 6.1 — Delivery**
```
Sophia → Human Operator:
- Sophia packages approved output
- Summary of who did what
- Quality score disclosed
- Limitations clearly stated
```

**Step 6.2 — Knowledge Promotion (if warranted)**
```
Institute Archivist:
- Reviews research output for knowledge-worthy items
- Formats items using Knowledge_Entry_Template.md
- Submits to Director
- Director submits to Sophia for Knowledge Base promotion
```

**Step 6.3 — Logging**
```
Sophia:
- Logs completed task in Logging.md format
- Updates session summary
```

---

## Timing Standards

| Phase | Maximum Duration |
|-------|-----------------|
| Phase 1 — Initiation | Before research begins |
| Phase 2 — Research | Defined in task brief |
| Phase 3 — Verification | 20% of research time |
| Phase 4 — Documentation | 10% of research time |
| Phase 5 — QC | 1 review cycle per session |
| Phase 6 — Delivery | Same session as approval |

---

## Error States

| Error | Response |
|-------|---------|
| Research question cannot be answered | Document why, return partial findings |
| Verification fails for critical claim | Flag as unverified, escalate to Sophia |
| Source contradictions unresolvable | Document both, label as contested |
| Two revision cycles without approval | Escalate to human operator |

---

## Connection to Other Documents

| Document | Relationship |
|----------|-------------|
| `02_Core/Research.md` | Research methodology used in Phase 2 |
| `02_Core/Verification.md` | Verification process used in Phase 3 |
| `01_Sophia/QualityControl.md` | QC process used in Phase 5 |
| `06_Templates/Research_Template.md` | Template used in Phase 4 |

---

*AION Foundation v0.1.0 — 05_Workflows/Research_Workflow.md*
