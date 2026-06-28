# Contribution Guide
## 09_Governance / Contribution_Guide.md

> *"AION grows through disciplined contribution — not through uncoordinated addition."*

---

## Overview

This guide explains how to contribute to the AION repository — whether you are a human developer or an AION agent proposing a change.

---

## What Can Be Contributed

| Contribution Type | Description |
|-------------------|-------------|
| New agent definition | A new specialist agent for an existing institute |
| New institute proposal | A proposal for a new institute (requires full governance process) |
| Knowledge base entry | A verified knowledge entry for `07_Knowledge/` |
| Bug fix | Correction of an error in an existing document |
| Improvement | Enhancement of an existing document |
| Template update | Improvement to a template in `06_Templates/` |
| Governance change | Change to policies or standards (highest scrutiny) |

---

## Contribution Process

### Step 1 — Fork and Branch
```
1. Fork the AION repository
2. Create a branch with a descriptive name:
   Format: [type]/[description]
   Examples:
     agent/turing-debugger
     knowledge/quantum-computing-basics
     fix/ethics-md-typo
     improvement/sophia-decision-engine
```

### Step 2 — Make Your Change
Follow all standards:
- Use the correct template from `06_Templates/`
- Follow naming conventions from `00_Constitution/Naming.md`
- Meet quality standards from `09_Governance/Quality_Standards.md`
- Verify all factual claims per `02_Core/Verification.md`

### Step 3 — Self-Review Checklist
Before submitting:

- [ ] Correct template used
- [ ] All metadata complete
- [ ] Version number assigned
- [ ] Status set to `Draft`
- [ ] All factual claims sourced
- [ ] No domain violations (content belongs in this institute/file)
- [ ] No naming convention violations
- [ ] CHANGELOG.md updated (for significant changes)

### Step 4 — Submit Pull Request

PR title format:
```
[Type] Brief description — [Institute if applicable]
Examples:
  [Agent] Herald — Hermes Institute Director definition
  [Knowledge] Quantum Computing Basics — Newton Institute
  [Fix] Ethics.md — corrected prohibited actions table
```

PR description must include:
- What you changed or added
- Why (what problem does this solve or what gap does it fill)
- Which documents you referenced
- Self-review checklist confirmation

### Step 5 — Review Process

1. Automated checks (template compliance, naming conventions)
2. Domain review (does this belong here?)
3. Quality review (meets standards?)
4. Ethics review for agent/institute proposals
5. Approval by repository maintainer

---

## Quality Bar

All contributions must meet a minimum score of **4.0** across the quality dimensions in `09_Governance/Quality_Standards.md`.

Contributions below 4.0 will be returned for revision with specific feedback.

---

## What We Do Not Accept

| Rejection Reason | Description |
|-----------------|-------------|
| Unverified claims | Factual claims without sources |
| Domain violations | Content that belongs in another institute |
| Template non-compliance | Not using the correct template |
| Naming violations | Not following `Naming.md` |
| Ethics violations | Content that violates `Ethics.md` |
| Duplicate content | Content that already exists |
| Speculation as fact | Unconfirmed claims presented as confirmed |

---

## Questions

If you are unsure whether a contribution is appropriate or how to structure it:
1. Open an issue describing the proposed contribution
2. Reference the relevant AION documents
3. Ask for guidance before investing significant time

---

*AION Foundation v0.1.0 — 09_Governance/Contribution_Guide.md*
