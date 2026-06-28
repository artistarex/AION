# Archive
## 08_Archive / README.md

> *"We do not delete. We preserve."*

---

## Overview

The AION Archive contains **deprecated documents, superseded versions, and historical records**.

All files in this folder are **read-only**.
No file in this folder is ever deleted.

---

## Archive Structure

Files are stored at their original path structure, prefixed with their deprecation version:

```
08_Archive/
└── [OriginalPath]/
    └── [filename]_deprecated_v[version].md
```

---

## Adding to the Archive

When a document is deprecated:
1. Copy to `08_Archive/[original_path]/[filename]_deprecated_v[old_version].md`
2. Add a deprecation header to the archived copy:
```
> ⚠️ ARCHIVED DOCUMENT
> Deprecated: [Date]
> Reason: Replaced by v[new_version]
> Current document: [path]
```
3. Update the live document to its new version
4. Log the deprecation in `02_Core/Logging.md`

---

## Current Archive Contents

*Empty at v0.1.0 — AION is beginning its history.*

---

*AION Foundation v0.1.0 — 08_Archive/README.md*
