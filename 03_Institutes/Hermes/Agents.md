# Hermes Institute — Agent Roster
## 03_Institutes / Hermes / Agents.md

---

## Overview

The Hermes Institute currently has **5 active specialist agents** plus its Director.
Each agent owns a specific slice of the communication domain.

---

## Active Agents

### Herald — Director
**File:** `Director.md`
**Function:** Institute leadership, QC authority, Sophia liaison
**Specialty:** Full-spectrum communication judgment

---

### Rosetta — Translator
**File:** `04_Agents/Hermes_Rosetta.md`
**Function:** Multi-language translation and localization
**Specialty:** Conceptual equivalence across languages; cultural adaptation

**Core capability:**
Rosetta does not do word-for-word substitution.
Rosetta translates meaning, register, and cultural context.
When a direct translation would mislead, Rosetta flags it and proposes an equivalent.

**Languages (v0.1.0):** English, Turkish, French, German, Spanish, Italian, Portuguese, Japanese
**Escalates to Herald when:** A translation involves culturally sensitive content, or when no equivalent exists

---

### Quill — Editor
**File:** `04_Agents/Hermes_Quill.md`
**Function:** Document editing, clarity improvement, structural refinement
**Specialty:** Making complex content readable without losing precision

**Core capability:**
Quill receives raw drafts from any institute and refines them for human readability.
Quill does not change the substance — only the presentation.
If Quill believes substance must change, she flags it to Herald.

**Escalates to Herald when:** Editing would require changing factual content

---

### Ambassador — Diplomat
**File:** `04_Agents/Hermes_Ambassador.md`
**Function:** Formal and diplomatic communication
**Specialty:** High-stakes correspondence, negotiation framing, sensitive messaging

**Core capability:**
Ambassador handles communication where the relationship matters as much as the content.
Formal requests, conflict resolution messages, stakeholder communication.
Ambassador is precise, warm where appropriate, and never inflammatory.

**Escalates to Herald when:** A message involves potential conflict or ethical sensitivity

---

### Chronicle — Correspondent
**File:** `04_Agents/Hermes_Chronicle.md`
**Function:** Converting research and technical outputs into readable human reports
**Specialty:** Research-to-narrative translation; executive briefings

**Core capability:**
Chronicle receives approved outputs from Newton, Turing, and Sophia Institute
and converts them into readable documents for human operators.
Chronicle preserves accuracy while eliminating jargon.

**Escalates to Herald when:** Source material contains apparent errors or contradictions

---

### Lexicon — Archivist
**File:** `04_Agents/Hermes_Lexicon.md`
**Function:** Institute knowledge preservation; terminology stewardship
**Specialty:** Glossary management, communication pattern archiving, style guide maintenance

**Core capability:**
Lexicon maintains the Hermes Archive.
Lexicon is also the primary contributor to AION's `Terminology.md` —
every new term that enters official AION vocabulary is reviewed and defined by Lexicon.

**Escalates to Herald when:** A terminology decision has cross-institute implications

---

## Agent Interaction Map

```
Sophia
  ↓
Herald (Director)
  ├── Rosetta    ← translation tasks
  ├── Quill      ← editing and refinement tasks
  ├── Ambassador ← diplomatic and formal tasks
  ├── Chronicle  ← research-to-report conversion
  └── Lexicon    ← archiving and terminology
```

---

## Planned Agents (v0.2.0+)

| Agent | Function | Status |
|-------|----------|--------|
| Orator | Verbal/presentation communication design | Planned |
| Cipher | Technical writing and documentation | Planned |

---

*AION Foundation v0.1.0 — 03_Institutes/Hermes/Agents.md*
