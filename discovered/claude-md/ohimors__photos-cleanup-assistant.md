---
name: ohimors__photos-cleanup-assistant
source: https://github.com/ohimors/photos-cleanup-assistant/blob/3066a0a281d61a75f1299d7e8601ecad7eb6b421/claude.MD
repo: ohimors/photos-cleanup-assistant
kind: claude-md
stars: 0
last_pushed: 2026-05-22T10:50:34Z
license: unknown
score: 8
domains: [browser-extensions, web-frontend, security]
tags: [chrome-extension, manifest-v3, privacy-first]
curated: 2026-06-15
curated_by: config-scout
---

# ohimors/photos-cleanup-assistant — claude-md

**Why it's worth keeping:** The 'Non-goals' and 'Why this exists' sections provide critical reasoning that prevents an AI from attempting impossible or prohibited automations. It also establishes clear technical constraints for data storage and permissions to ensure compliance.

**Summary:** A highly structured instruction set for a Chrome extension that defines strict product boundaries and security guardrails.

**Source credibility:** Low social proof (0 stars), but demonstrates high professional maturity in its documentation architecture.

**Recency:** Current; aligns with modern Manifest V3 standards.

**Source:** [ohimors/photos-cleanup-assistant/claude.MD](https://github.com/ohimors/photos-cleanup-assistant/blob/3066a0a281d61a75f1299d7e8601ecad7eb6b421/claude.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# claude.md — Photos Cleanup Assistant (Chrome Extension)

## Product name
Photos Cleanup Assistant

## One-line description
A privacy-first Chrome extension that helps users *identify* (select all photos that match criteria) Google Photos items to clean up (date-range batches, duplicates, large videos), then guides them through a safe, manual delete workflow in Google Photos.

## Why this exists
Google Photos does not provide a public API to delete media items from a user’s library. The official APIs support limited album management (e.g., removing media items from albums under constraints) but not true library deletion. Therefore, this product is intentionally designed as a *review + guided cleanup* tool, not an automated deletion bot. (Avoids high-risk automation patterns and aligns with Chrome Web Store policies.) 

## Goals (must-haves)
1. Help users find media candidates by:
   - Date range (e.g., “Jan 1–Jan 31, 2022”)
   - Media type (photo/video)
   - Large items (e.g., videos above X MB) — best-effort via UI metadata or local heuristics
   - Duplicates (perceptual hash on downloaded thumbnails where possible; see constraints)
2. Build a “Review Queue”:
   - User creates a
```

</details>
