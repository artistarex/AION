# Version Control
## 09_Governance / Version_Control.md

---

## Overview

This document defines the versioning standards for all AION documents and the repository itself.

Version control is not bureaucracy — it is the mechanism that lets AION learn from its history.

---

## Repository Versioning

AION uses semantic versioning: `v[MAJOR].[MINOR].[PATCH]`

| Component | Triggers Increment |
|-----------|-------------------|
| **MAJOR** | Architectural change, breaking change, new AION version milestone |
| **MINOR** | New institute, new agent, new workflow, new knowledge domain |
| **PATCH** | Bug fix, correction, small update, clarification |

**Current:** v0.1.0 — Foundation

---

## Document Versioning

Every document carries its own version number, independent of the repository version.

| Component | Triggers Increment |
|-----------|-------------------|
| **MAJOR** | Fundamental rethinking of the document's purpose or content |
| **MINOR** | Significant addition or change to content |
| **PATCH** | Correction, clarification, small addition |

**Every document must have:**
```
**Version:** v[x.x.x]
**Status:** Draft / Review / Approved / Deprecated / Archived
**Last Updated:** [Date]
```

---

## Version Increment Rules

**Never overwrite** — create a new version.
Previous versions are:
- Documented in the document's own changelog section
- Archived in `08_Archive/` when deprecated

**Always increment when:**
- Any content changes (patch minimum)
- Status changes from Draft to Review to Approved (patch)

**Never increment for:**
- Formatting fixes with no content change
- Metadata updates (date, author) without content change

---

## Status Progression

```
Draft → Review → Approved → Deprecated → Archived
```

| Status | Meaning | Who Can Write |
|--------|---------|--------------|
| Draft | Being written | Authoring agent |
| Review | Under QC review | Read-only (reviewer adds notes) |
| Approved | Passed QC, official | Read-only (new version to change) |
| Deprecated | Replaced by newer version | Read-only |
| Archived | Moved to 08_Archive/ | Read-only |

---

## CHANGELOG.md Maintenance

The repository `CHANGELOG.md` is updated with every significant change:

```markdown
## [Version] — Release Name
### Added
- [New items]
### Changed
- [Modified items]
### Fixed
- [Corrected items]
### Deprecated
- [Items superseded]
```

Minor fixes may be batched into one CHANGELOG entry.
Major changes get their own entry.

---

## 08_Archive/ Management

When a document is deprecated:
1. Copy to `08_Archive/[original_path]/[filename]_v[old_version].md`
2. Add deprecation note to the top of the archived file
3. Update the original file to new version
4. Log the deprecation

```
# ARCHIVED DOCUMENT
- **Archived:** [Date]
- **Reason:** Replaced by v[new version]
- **Current document:** [path to current version]
---
[Original content below]
```

---

*AION Foundation v0.1.0 — 09_Governance/Version_Control.md*
