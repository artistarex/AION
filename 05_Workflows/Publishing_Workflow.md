# Publishing Workflow
## 05_Workflows / Publishing_Workflow.md

---

## Overview

This workflow defines how AION outputs move from "Approved" status to final delivery
and knowledge archiving.

Publishing is the last step — but not the least important.
How an output is packaged and delivered shapes whether it is actually useful.

---

## Trigger

This workflow begins when Sophia approves an output (QC score ≥ 4.0).

---

## Publishing Steps

### Step 1 — Delivery Package Assembly

Sophia assembles the delivery package:

```
Delivery Package Contents:
├── Primary output document (Approved)
├── Executive summary (if not included in output)
├── Attribution note (who produced what)
├── Quality score disclosure (optional but encouraged)
└── Limitations note (always included)
```

### Step 2 — Format Selection

| Audience | Format |
|---------|--------|
| Human operator (general) | Markdown or formatted report |
| Human operator (technical) | Technical spec format |
| Human operator (executive) | Briefing format (max 1 page summary) |
| Cross-institute reference | Full document with all metadata |

### Step 3 — Delivery

Sophia delivers to human operator with a delivery note:

```
Delivery Note Format:
FROM: Sophia | Executive
TO: [Operator]
TASK_ID: [ID]
SUBJECT: [Task title] — Output Delivered

This output was produced by:
- [Institute(s)] — [Component(s)]

Quality score: [X.X/5.0]
Verification level: L[1/2/3]

Key limitations: [1-2 sentences]

Full output attached/below.
```

### Step 4 — Knowledge Promotion Review

After delivery, Sophia reviews the output for Knowledge Base promotion:

**Promote if:**
- Output contains verified facts not yet in Knowledge Base
- Output contains a reusable methodology or framework
- Output answers a question likely to recur

**Process:**
1. Sophia identifies promotable items
2. Routes to originating institute Archivist
3. Archivist formats using `Knowledge_Entry_Template.md`
4. Archivist → Director → Sophia → Global Knowledge Base

### Step 5 — Task Closure

Sophia closes the task:
1. Task logged as complete in `02_Core/Logging.md`
2. Session summary updated
3. Any follow-up tasks identified and queued

---

## Connection to Other Documents

| Document | Relationship |
|----------|-------------|
| `01_Sophia/QualityControl.md` | QC must pass before this workflow runs |
| `06_Templates/Report_Template.md` | Format used for final delivery |
| `07_Knowledge/` | Destination for promoted knowledge |
| `02_Core/Logging.md` | Task closure logging |

---

*AION Foundation v0.1.0 — 05_Workflows/Publishing_Workflow.md*
