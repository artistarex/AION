# AION
## Artificial Intelligence Omni Network

> **"One AI should not know everything. Many experts must cooperate."**

---

![Version](https://img.shields.io/badge/version-0.3.0-gold)
![Institutes](https://img.shields.io/badge/institutes-7-blue)
![Agents](https://img.shields.io/badge/agents-63-purple)
![Status](https://img.shields.io/badge/status-Active-green)
![License](https://img.shields.io/badge/license-MIT-gray)

---

## Overview

AION is a **modular multi-agent operating system** — a network of specialized AI agents organized into independent institutes, coordinated by a central executive intelligence named **Sophia**.

Instead of one general-purpose AI doing everything, AION distributes knowledge, reasoning, verification, planning, and execution across **7 dedicated expert institutes** with **63 specialist agents**.

---

## Architecture

```
Human Operator
      ↓
  Sophia (Executive Intelligence)
      ↓
  Core Systems (Memory · Knowledge Graph · Verification · Logging)
      ↓
  Institute Network
      ├── Hermes Institute     — Communication · Translation · Language · Docs
      ├── Newton Institute     — Science · Research · Verification · Analytics
      ├── Turing Institute     — Technology · Engineering · Code · Security
      ├── Sophia Institute     — Philosophy · Ethics · Strategy · Psychology
      ├── DaVinci Studio       — Creative · Design · Motion · Video · UX
      ├── Agora Institute      — Business · Finance · Legal · Operations
      └── Mercury Institute    — Marketing · Growth · SEO · PR · Social
      ↓
  63 Specialist Agents
      ↓
  Knowledge Base
```

---

## The Seven Institutes

| Institute | Domain | Director | Agents |
|-----------|--------|----------|--------|
| **Hermes** | Communication, Translation, Technical Docs | Herald | 7 |
| **Newton** | Science, Research, Verification, Analytics | Archimedes | 10 |
| **Turing** | Technology, Engineering, Code, Security | Lovelace | 12 |
| **Sophia Institute** | Philosophy, Ethics, Strategy, Psychology | Athena | 10 |
| **DaVinci Studio** | Creative, Design, Motion, Video, UX | Muse | 11 |
| **Agora Institute** | Business, Finance, Legal, Operations | Strategos | 10 |
| **Mercury Institute** | Marketing, Growth, SEO, PR, Social | Pulse | 7 |

---

## Core Philosophy

| Principle | Description |
|-----------|-------------|
| **Specialization** | Each agent has one defined domain |
| **Verification** | Every claim must be traced to a source |
| **Transparency** | All reasoning is documented |
| **Preservation** | Knowledge is version-controlled |
| **Quality** | Measurable standards at every step |
| **Cooperation** | Institutes collaborate via defined protocols |

---

## Running AION

### Option A — Claude Project (simplest)
1. Copy `AION_SYSTEM_PROMPT_v0.3.md` contents
2. Create a new Claude Project at claude.ai
3. Paste into Project Instructions
4. Every conversation in that project runs through Sophia

### Option B — API (Python)
```bash
pip install anthropic
export ANTHROPIC_API_KEY="sk-ant-..."
python aion_api.py
```

---

## Repository Structure

```
AION/
├── README.md
├── CHANGELOG.md
├── ROADMAP.md
├── DIRECTORY.md
│
├── 00_Constitution/        # Vision, Mission, Principles, Rules, Ethics, Naming, Terminology
├── 01_Sophia/              # Executive Intelligence — Decision, Coordination, QC
├── 02_Core/                # Memory, KnowledgeGraph, Verification, Communication, Logging
│
├── 03_Institutes/
│   ├── Hermes/             # Institute.md · Director.md · Agents.md · Protocols.md · Archive.md
│   ├── Newton/
│   ├── Turing/
│   ├── Sophia/
│   ├── DaVinci/
│   ├── Agora/              # New in v0.3.0
│   └── Mercury/            # New in v0.3.0
│
├── 04_Agents/              # 63 agent definition files
├── 05_Workflows/           # Research, Validation, Publishing, Emergency protocols
├── 06_Templates/           # Agent, Institute, Research, Report, Knowledge Entry
├── 07_Knowledge/           # Verified knowledge base — 6 domains
├── 08_Archive/             # Deprecated documents
└── 09_Governance/          # Quality standards, Review policy, Contribution guide
```

---

## Versioning

| Version | Status | Description |
|---------|--------|-------------|
| v0.1.0 | ✅ Released | Foundation — Constitution, Sophia, Core, 5 institutes |
| v0.2.0 | ✅ Released | +5 agents: Oracle, Darwin, Shannon, Cipher, Stage |
| v0.3.0 | ✅ Current | +34 agents, +2 institutes (Agora, Mercury) — 63 total |
| v1.0.0 | 🔄 Planned | Python runtime — CrewAI / LangGraph implementation |

See [`ROADMAP.md`](ROADMAP.md) for the full plan.

---

## Contributing

See [`09_Governance/Contribution_Guide.md`](09_Governance/Contribution_Guide.md).

All contributions must meet the quality standard defined in [`09_Governance/Quality_Standards.md`](09_Governance/Quality_Standards.md).

---

## License

MIT License. See [`LICENSE.md`](LICENSE.md).

---

*AION v0.3.0 — Built by [Artista](https://github.com/artistarex) · 7 institutes · 63 agents · 144 documents*
