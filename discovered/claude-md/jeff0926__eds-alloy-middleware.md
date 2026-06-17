---
name: jeff0926__eds-alloy-middleware
source: https://github.com/jeff0926/eds-alloy-middleware/blob/0ddf2bcd801670693ef01696ddfa85ab1b038f1e/CLAUDE.md
repo: jeff0926/eds-alloy-middleware
kind: claude-md
stars: 0
last_pushed: 2026-05-15T15:22:21Z
license: unknown
score: 9
domains: [backend-api, data-ingestion]
tags: [node-express, sqlite, architecture-boundaries, middleware]
curated: 2026-06-15
curated_by: config-scout
---

# jeff0926/eds-alloy-middleware — claude-md

**Why it's worth keeping:** The 'Hard Rules' and 'Decision Defaults' sections are elite examples of scope-creep prevention, while the 'Alloy -> Middleware Trick' provides essential domain-specific logic that an AI wouldn't otherwise know.

**Summary:** A highly structured instruction set for a Node/Express middleware that captures Adobe Alloy.js signals into SQLite. It strictly enforces architectural boundaries to prevent code-leakage from a related project.

**Source credibility:** Low social proof (0 stars), but the technical depth suggests a highly competent individual developer.

**Recency:** Highly current; fits perfectly with Claude Code's need for explicit architectural boundaries and decision-making frameworks.

**Source:** [jeff0926/eds-alloy-middleware/CLAUDE.md](https://github.com/jeff0926/eds-alloy-middleware/blob/0ddf2bcd801670693ef01696ddfa85ab1b038f1e/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — eds-alloy-middleware

**Project:** EDS + Alloy + Capture Middleware (standalone)
**Owner:** 864zeros LLC / Jeff Conn
**Relationship to AETHER:** None. AETHER is a separate project at `C:\Users\I820965\dev\aether\`. Do not import, reference, or scaffold for AETHER in this repo.

---

## What This Project Is

A standalone edge-publishing site that demonstrates Adobe EDS (Franklin) free-tier deployment paired with Alloy.js client-side data collection — without an Adobe Experience Platform (AEP) license. Behavioral signals captured by Alloy.js are POSTed to a local middleware that normalizes and stores them.

This project intentionally has **two snap-in seams** for a future system (AETHER) to plug into:

| Seam | Direction | Mechanism |
|---|---|---|
| Content ingress | Inbound | Markdown files in `/site/content/` consumed by EDS rendering pipeline |
| Signal egress | Outbound | SQLite event stream + REST endpoint at `/events` |

Both seams must remain **dormant but architected** in Phase 1. Do not build AETHER integration logic. Do build the seams cleanly.

---

## Hard Rules

1. No AETHER code, dependencies, or imports. This repo ships standalone.
2. Default EDS blocks
```

</details>
