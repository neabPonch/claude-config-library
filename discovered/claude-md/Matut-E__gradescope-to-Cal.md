---
name: Matut-E__gradescope-to-Cal
source: https://github.com/Matut-E/gradescope-to-Cal/blob/5d52a260ddfcf55727ffd737c51ba4f7faa55344/Claude.md
repo: Matut-E/gradescope-to-Cal
kind: claude-md
stars: 3
last_pushed: 2026-01-16T00:32:36Z
license: mit
score: 9
domains: [browser-extensions, web-frontend]
tags: [architecture, data-schema, bug-prevention]
curated: 2026-06-16
curated_by: config-scout
---

# Matut-E/gradescope-to-Cal — claude-md

**Why it's worth keeping:** The inclusion of 'CRITICAL' warnings about historical bugs prevents regressions. Providing exact schema examples ensures the AI writes correct, production-ready integration code without hallucination.

**Summary:** Provides an exhaustive technical blueprint including specific JSON object structures for API calls and internal storage schemas. It serves as both a high-level architecture guide and a rigorous data specification.

**Source credibility:** Small personal project with moderate activity.

**Recency:** Recent (last pushed 5 months ago).

**Source:** [Matut-E/gradescope-to-Cal/Claude.md](https://github.com/Matut-E/gradescope-to-Cal/blob/5d52a260ddfcf55727ffd737c51ba4f7faa55344/Claude.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Gradescope to Cal** is an open-source, MIT-licensed browser extension that automatically syncs UC Berkeley Gradescope assignments to Google Calendar. Published on the Chrome Web Store, it helps students stay organized by creating calendar events for all upcoming assignments.

**Key characteristics**:
- **Open source**: MIT licensed, publicly available
- **Automatic sync**: First-time sync + manual sync + 24-hour auto-sync + smart sync on extraction
- **Production version**: v2.0.1 on Chrome Web Store
- **Privacy-first**: Zero-server architecture, all processing in browser

## Core Features

This extension provides:

1. **Assignment Extraction**: Extracts upcoming assignments from Gradescope dashboard and course pages
2. **Google Calendar Integration**: OAuth 2.0 authentication and Calendar API v3 integration
3. **Four Sync Mechanisms**:
   - **First-Time Sync**: Immediate sync on first authentication (if assignments already extracted)
   - **Manual Sync**: User-triggered sync via "Sync to Calendar" button
   - **24-Hour Auto-Sync**: Scheduled b
```

</details>
