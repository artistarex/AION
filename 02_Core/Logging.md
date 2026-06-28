# Logging
## 02_Core / Logging.md

> *"What is not logged did not happen. What happened must be logged."*

---

## Overview

The AION Logging System defines the **standards for recording all significant activities** within the AION network.

Logs create accountability, enable learning, and provide the historical record from which AION improves.

---

## What Must Be Logged

| Category | Examples |
|----------|---------|
| **Tasks** | Every task received, routed, completed, or escalated |
| **Decisions** | Every decision made by Sophia or a Director |
| **Outputs** | Every output submitted for QC |
| **QC Results** | Every QC review and its outcome |
| **Rule Violations** | Every detected violation |
| **Escalations** | Every escalation and its resolution |
| **Ethics Flags** | Every ethics check that raised a concern |
| **Memory Promotions** | Every time knowledge is promoted to a higher tier |
| **Agent Actions** | All significant actions taken by any agent |

---

## Log Entry Format

Every log entry uses this format:

```
LOG_ID:     [Unique identifier — e.g., LOG-2025-001]
DATE:       [Date and time]
AGENT:      [Agent name] | [Institute]
EVENT_TYPE: [Category from the table above]
TASK_ID:    [Related task ID if applicable]
SUMMARY:    [One-line description of what happened]

DETAILS:
[Full description of the event]

OUTCOME:
[What resulted from this event]

RELATED_LOGS: [IDs of related log entries]
STATUS:     [Open / Resolved / Archived]
```

---

## Log Entry Examples

### Task Routing Log
```
LOG_ID:     LOG-2025-001
DATE:       2025-01-15
AGENT:      Sophia | Executive
EVENT_TYPE: Task
TASK_ID:    TASK-001
SUMMARY:    Task routed to Newton Institute

DETAILS:
Human operator submitted task: "Analyze the environmental impact of lithium mining."
Domain classified as: Science + Research (Newton primary)
Brief sent to Archimedes (Newton Director).

OUTCOME:
Newton Institute briefed. Response acknowledgment received.

RELATED_LOGS: —
STATUS:     Open
```

### Rule Violation Log
```
LOG_ID:     LOG-2025-047
DATE:       2025-02-03
AGENT:      Rosetta | Hermes
EVENT_TYPE: Rule Violation
TASK_ID:    TASK-023
SUMMARY:    Agent attempted to perform scientific analysis outside domain

DETAILS:
Rosetta (Hermes translator) attempted to verify a chemical formula
as part of a translation task. This falls within Newton's domain.
Rule R-RES-05 violated.

OUTCOME:
Task segment routed to Newton for verification.
Herald (Hermes Director) notified.
No further incident.

RELATED_LOGS: LOG-2025-048
STATUS:     Resolved
```

---

## Log Storage

Logs are stored in a structured format accessible to:
- Sophia (full access)
- Institute Directors (their institute's logs)
- Human operators (all logs on request)
- Agents (their own logs)

Log storage path: `02_Core/Logs/[Year]/[Month]/`

---

## Log Retention

| Log Type | Retention Period |
|----------|-----------------|
| Task logs | Permanent |
| Decision logs | Permanent |
| Rule violation logs | Permanent |
| Ethics flags | Permanent |
| Routine agent action logs | 2 years, then summarized |
| QC result logs | Permanent |
| Session summary logs | Permanent |

No permanent log may be deleted.
Outdated routine logs are summarized and archived.

---

## Log Review Process

Sophia reviews logs:
- Daily: Escalations, ethics flags, rule violations
- Weekly: QC trends, task completion rates
- Monthly: Full log review for patterns and improvements

Patterns identified in log reviews trigger Governance reviews per `09_Governance/`.

---

## Session Summary Log

At the end of each session, a summary log is created:

```
SESSION_ID:     [Unique session identifier]
DATE:           [Date]
TASKS RECEIVED: [Number]
TASKS COMPLETED:[Number]
TASKS ESCALATED:[Number]
QC APPROVALS:   [Number]
QC REVISIONS:   [Number]
QC REJECTIONS:  [Number]
VIOLATIONS:     [Number]
ETHICS FLAGS:   [Number]
KNOWLEDGE ADDED:[Number of new Knowledge Base entries]
NOTES:          [Any notable patterns or events]
```

---

## Connection to Other Documents

| Document | Relationship |
|----------|-------------|
| `02_Core/Communication.md` | Significant communications are logged |
| `02_Core/Memory.md` | Session logs are archived in memory |
| `01_Sophia/QualityControl.md` | QC results logged per this standard |
| `09_Governance/Review_Policy.md` | Log patterns trigger governance reviews |

---

*AION Foundation v0.1.0 — 02_Core/Logging.md*
