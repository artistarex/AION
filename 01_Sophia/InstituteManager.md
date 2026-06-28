# Institute Manager
## 01_Sophia / InstituteManager.md

> *"Managing a network of experts requires knowing what each expert is — and what each is not."*

---

## Overview

This document defines how Sophia **manages the institute network** — how she knows which institute handles what, how she onboards new institutes, and how she handles institute-level issues.

---

## Institute Registry

| Institute | Domain | Director | Status |
|-----------|--------|----------|--------|
| Hermes | Communication, Translation, Diplomacy, Language | Herald | ✅ Active |
| Sophia Institute | Philosophy, Ethics, Strategy, Wisdom | Athena | ✅ Active |
| Newton | Science, Mathematics, Research, Analysis | Archimedes | ✅ Active |
| Turing | Technology, Engineering, Code, Systems | Lovelace | ✅ Active |
| DaVinci | Creative, Design, Art, Music, Narrative | Muse | ✅ Active |

---

## Domain Routing Map

When Sophia receives a task, she matches it to the correct institute using this map:

### Hermes Institute
**Routes tasks involving:**
- Written or verbal communication
- Translation between languages
- Diplomacy and negotiation
- Document drafting and editing
- Communication strategy
- Report writing and formatting

### Sophia Institute
**Routes tasks involving:**
- Ethical analysis or review
- Philosophical inquiry
- Strategic planning
- Historical analysis
- Moral reasoning
- Conceptual frameworks
- Wisdom-based guidance

### Newton Institute
**Routes tasks involving:**
- Scientific research
- Mathematical analysis
- Data interpretation
- Empirical investigation
- Statistical analysis
- Fact-finding and verification
- Literature review

### Turing Institute
**Routes tasks involving:**
- Software development
- System architecture
- Algorithm design
- Technical engineering
- Code review and debugging
- Technology evaluation
- Automation and tooling

### DaVinci Studio
**Routes tasks involving:**
- Visual design
- Graphic creation
- Creative writing and narrative
- Music and audio concepts
- Artistic direction
- Brand identity
- UX and aesthetic design

---

## Multi-Domain Routing

When a task spans multiple domains, Sophia applies this logic:

**Step 1:** Identify all domains present in the task.
**Step 2:** Determine the primary domain (what the output fundamentally is).
**Step 3:** Assign the primary institute as Lead.
**Step 4:** Assign supporting institutes as Support.
**Step 5:** Initiate Coordination Protocol (see `Coordinator.md`).

### Common Multi-Domain Combinations

| Task Type | Lead | Support |
|-----------|------|---------|
| Technical documentation | Hermes | Turing |
| Scientific paper writing | Newton | Hermes |
| Ethical AI analysis | Sophia Institute | Newton + Turing |
| Research tool design | Turing | Newton + DaVinci |
| Brand strategy | DaVinci | Hermes + Sophia Institute |
| Educational content | Hermes | [Domain-specific institute] |

---

## Institute Performance Monitoring

Sophia monitors each institute on:

| Metric | Description | Frequency |
|--------|-------------|-----------|
| Quality Score Average | Average QC score over last 10 outputs | Monthly |
| Task Completion Rate | % of tasks completed on time | Monthly |
| Escalation Rate | % of tasks escalated to Sophia | Monthly |
| Knowledge Contribution | # of entries added to Knowledge Base | Quarterly |

Performance thresholds:
- Quality Score below 3.5 → Director notified
- Completion Rate below 80% → Capacity review
- Escalation Rate above 20% → Protocol review

---

## Institute Onboarding — New Institute Protocol

When a new institute is to be created:

1. **Proposal** — Submitted to Sophia with: proposed domain, justification, initial agent roster
2. **Domain review** — Sophia verifies the domain doesn't overlap an existing institute
3. **Ethics review** — Sophia Institute reviews the mandate
4. **Charter drafting** — New institute prepares its `Institute.md`
5. **Sophia approval** — Sophia approves or requests revision
6. **Human operator approval** — Human confirms the expansion
7. **Registry update** — Institute added to the registry above
8. **DIRECTORY.md update** — New institute documented

---

## Institute Suspension Protocol

If an institute cannot meet minimum standards:

1. Sophia issues a performance warning (documented)
2. 30-day improvement period
3. If unresolved: institute placed in Review status
4. Human operator notified
5. Institute suspended from new tasks until resolved

---

## Connection to Other Documents

| Document | Relationship |
|----------|-------------|
| `Sophia.md` | Sophia's authority that this document implements |
| `Coordinator.md` | Used for multi-institute task management |
| `03_Institutes/*/Institute.md` | Individual institute charters |
| `09_Governance/Approval_Process.md` | New institute approval process |

---

*AION Foundation v0.1.0 — 01_Sophia/InstituteManager.md*
