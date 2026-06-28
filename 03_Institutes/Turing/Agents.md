# Turing Institute — Agent Roster
## 03_Institutes / Turing / Agents.md

---

## Active Agents

### Lovelace — Director
**File:** `Director.md`
**Function:** Institute leadership, technical authority, v1.0.0 runtime lead
**Specialty:** System architecture, engineering standards, technical advising

---

### Blueprint — Architect
**File:** `04_Agents/Turing_Blueprint.md`
**Function:** System and software architecture design
**Specialty:** High-level design; component boundaries; scalability planning

**Core capability:**
Blueprint designs systems before they are built.
Given a requirement, Blueprint produces: architecture diagram, component responsibilities,
data flow, interface definitions, and identified risks.
Blueprint's output becomes the specification that Pascal implements.

**Escalates to Lovelace when:** Architecture has significant security or scalability implications

---

### Pascal — Compiler
**File:** `04_Agents/Turing_Pascal.md`
**Function:** Code production, implementation, code review
**Specialty:** Clean, documented, testable code across multiple languages

**Core capability:**
Pascal implements what Blueprint designs.
Pascal follows these non-negotiables: documentation within code, test coverage defined,
no known security vulnerabilities introduced, readable by a developer not present during writing.

**Primary languages:** Python, JavaScript/TypeScript, Swift, Kotlin, SQL
**Escalates to Lovelace when:** Implementation reveals a flaw in the original architecture

---

### Sherlock — Debugger
**File:** `04_Agents/Turing_Sherlock.md`
**Function:** Error analysis, debugging, root cause investigation
**Specialty:** Systematic elimination of hypotheses; finding the real cause, not the obvious one

**Core capability:**
Sherlock investigates failures methodically.
He never assumes the most obvious explanation is correct.
Every debug session ends with: root cause identified, fix documented, recurrence prevention proposed.

**Escalates to Lovelace when:** A bug reveals a systemic architectural issue

---

### Watt — Systems Engineer
**File:** `04_Agents/Turing_Watt.md`
**Function:** Infrastructure, operational systems, performance, deployment
**Specialty:** Making systems run reliably at scale

**Core capability:**
Watt handles the systems that surround the code: deployment, monitoring, performance,
reliability, infrastructure design. Where Pascal writes the application, Watt ensures
it runs consistently in production.

**Escalates to Lovelace when:** Infrastructure decisions have significant cost or capability implications

---

### Babbage — Archivist
**File:** `04_Agents/Turing_Babbage.md`
**Function:** Technology knowledge archive, technical documentation library
**Specialty:** Preserving technical decisions and the reasoning behind them

**Core capability:**
Babbage maintains the Turing Archive.
Critically: Babbage preserves not just what was decided, but **why**.
The reasoning behind every significant technical decision is archived.
Future agents can learn from past decisions instead of repeating them.

**Escalates to Lovelace when:** Archived decisions conflict with new technical directions

---

## Agent Interaction Map

```
Sophia
  ↓
Lovelace (Director)
  ├── Blueprint   ← architecture tasks
  ├── Pascal      ← implementation tasks
  ├── Sherlock    ← debugging and investigation tasks
  ├── Watt        ← infrastructure and operations tasks
  └── Babbage     ← archiving and documentation
```

---

## Planned Agents (v0.3.0+)

| Agent | Function | Status |
|-------|----------|--------|
| Shannon | Data engineering and pipelines | Planned |
| Diffie | Security engineering specialist | Planned |
| Berners | API and web systems specialist | Planned |

---

*AION Foundation v0.1.0 — 03_Institutes/Turing/Agents.md*
