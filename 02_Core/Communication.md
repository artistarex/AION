# Communication
## 02_Core / Communication.md

> *"In a network of experts, communication is not a courtesy — it is an infrastructure."*

---

## Overview

The AION Communication Layer defines the **protocols, formats, and channels** through which agents and institutes exchange information.

All inter-agent and inter-institute communication follows this document.

---

## Communication Channels

| Channel | Used For | Direction |
|---------|----------|-----------|
| **Sophia ↔ Director** | Task routing, status, decisions | Bidirectional |
| **Director ↔ Agent** | Task assignment, review, feedback | Bidirectional |
| **Agent ↔ Agent (same institute)** | Collaboration within institute | Bidirectional |
| **Institute ↔ Institute** | Cross-domain collaboration | Via Sophia only |
| **AION → Human Operator** | Final output delivery | Outbound |
| **Human Operator → AION** | Task input, instructions | Inbound to Sophia |

**Critical Rule:** Institutes do not communicate directly with each other.
All cross-institute communication passes through Sophia.

---

## Message Format

Every formal AION message follows this format:

```
FROM:    [Agent/Role Name] | [Institute]
TO:      [Agent/Role Name] | [Institute]
TYPE:    [Message Type]
TASK_ID: [Task identifier if applicable]
DATE:    [Date]

---

SUBJECT: [One-line description]

BODY:
[Message content]

---

ACTION REQUIRED: [Yes/No]
DEADLINE: [Date/Time or N/A]
RESPONSE TO: [Previous message ID or N/A]
```

---

## Message Types

| Type | Usage |
|------|-------|
| `BRIEF` | Task assignment from Sophia to Director |
| `REPORT` | Output submission from institute to Sophia |
| `REQUEST` | Information request between agents |
| `UPDATE` | Progress update |
| `REVIEW` | QC feedback from Sophia to institute |
| `DECISION` | Governance decision from Sophia |
| `ESCALATION` | Escalation to a higher authority |
| `ALERT` | Urgent notification |
| `ACKNOWLEDGMENT` | Confirmation of receipt |

---

## Communication Standards

### Clarity
Every message must be understood by the recipient without clarification.
If you are not certain the message is clear, it is not ready to send.

### Completeness
A message that requires follow-up for missing information is an incomplete message.
Include everything the recipient needs to act.

### Timeliness
Acknowledgments: within the same session.
Routine responses: within the defined task timeline.
Escalations: immediately.

### Tone
All AION communication is:
- Professional
- Neutral
- Precise
- Free of emotional language

### Documentation
All significant messages are logged per `Logging.md`.

---

## Acknowledgment Protocol

Every message that requires a response must be acknowledged.

**Acknowledgment format:**
```
ACKNOWLEDGMENT
FROM: [Recipient]
TO: [Sender]
MESSAGE REF: [Original message reference]
STATUS: Received and understood / Received — clarification needed
CLARIFICATION: [If needed — specific question]
```

If a Director does not acknowledge a Sophia brief within the session, Sophia follows up.
If still no response, Sophia escalates.

---

## Escalation Communication

Escalation messages have highest priority:

```
FROM:    [Agent/Role] | [Institute]
TO:      [Sophia / Director / Human Operator]
TYPE:    ESCALATION
PRIORITY: HIGH

SITUATION: [Describe the situation]
REASON FOR ESCALATION: [Why this cannot be resolved at current level]
ETHICAL CONCERN: [Yes/No — if yes, describe]
RECOMMENDED ACTION: [What the escalating agent recommends]
AWAITING: [What decision is needed]
```

---

## Communication Failures

If an expected communication is not received:

1. Wait one follow-up interval
2. Send a follow-up message (reference original)
3. If still no response: escalate to the next authority level
4. Log the failure in `Logging.md`

---

## Connection to Other Documents

| Document | Relationship |
|----------|-------------|
| `Logging.md` | All significant communications are logged |
| `01_Sophia/Coordinator.md` | Sophia uses this system to coordinate institutes |
| `05_Workflows/Research_Workflow.md` | Communication steps within research |
| `00_Constitution/Rules.md` | R-COM rules derived from this document |

---

*AION Foundation v0.1.0 — 02_Core/Communication.md*
