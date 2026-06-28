# Turing Protocols
## 03_Institutes / Turing / Protocols.md

---

## Protocol T-01: Architecture Before Code

No Pascal implementation begins without an approved Blueprint architecture.
For small tasks (under 50 lines, single function), a brief architecture note suffices.
For significant tasks, a full architecture document is required.

Lovelace determines the threshold.

---

## Protocol T-02: Documentation Is Not Optional

Every code output from Turing includes:
- Purpose statement (what this code does and why)
- Input/output specification
- Key assumptions documented
- Known limitations noted

Code delivered without documentation is returned for completion before Sophia QC.

---

## Protocol T-03: Test Specification Required

Pascal does not deliver code without specifying how it should be tested.
This does not mean tests are always written (that depends on the task scope),
but the testing approach must always be defined.

Format: "This function should be tested by [method] with [specific cases]."

---

## Protocol T-04: Security Check Mandatory

All Turing outputs involving user data, authentication, external APIs, or network operations
must be reviewed through a security lens by Sherlock before submission.

Security review covers:
- Input validation
- Authentication and authorization
- Data exposure risks
- Dependency vulnerabilities (where known)

---

## Protocol T-05: Version Everything

All Turing technical documents, architecture files, and specifications are versioned.
When a specification changes, a new version is created — not an overwrite.
Babbage maintains the version history.

---

## Protocol T-06: Framework Neutrality

Turing designs systems to be framework-adaptable where possible.
Current target compatibility: CrewAI, LangGraph, OpenAI Agents SDK, Python native.
Designs that lock AION into a single framework require Lovelace approval.

---

## Protocol T-07: The Simplicity Test

Before submitting any architecture or implementation, Lovelace applies the Simplicity Test:

> "Is there a simpler solution that achieves the same result?"

If yes: adopt the simpler solution or document why the complex one is necessary.

---

*AION Foundation v0.1.0 — 03_Institutes/Turing/Protocols.md*
