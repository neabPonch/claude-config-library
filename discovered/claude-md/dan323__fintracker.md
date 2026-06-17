---
name: dan323__fintracker
source: https://github.com/dan323/fintracker/blob/226d6e14d01fb425dbaacf4de3feb01023502936/CLAUDE.md
repo: dan323/fintracker
kind: claude-md
stars: 1
last_pushed: 2026-06-12T21:24:19Z
license: other
score: 9
domains: [web-frontend, react]
tags: [react, typescript, vite, documentation-template]
curated: 2026-06-15
curated_by: config-scout
---

# dan323/fintracker — claude-md

**Why it's worth keeping:** Includes 'Common Development Tasks' workflows (e.g., adding components) and specific command templates for running individual tests, which is highly effective for agentic coding.

**Summary:** A comprehensive blueprint for a React/TypeScript SPA that outlines data flow, component responsibilities, and specific extension patterns.

**Source credibility:** Low star count, but the documentation depth indicates a high-quality or well-structured project.

**Recency:** Highly current, utilizing React 19 and Node 22.

**Source:** [dan323/fintracker/CLAUDE.md](https://github.com/dan323/fintracker/blob/226d6e14d01fb425dbaacf4de3feb01023502936/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Quick Reference

**Development Setup**
- Node.js 22+ required (check `.nvmrc`); use `nvm` or `nvm-windows` for version management
- Install: `npm install`
- Start dev server: `npm start` (runs on http://localhost:5173 with Vite)
- Tests: `npm test` (Vitest with jsdom environment)
- Build: `npm run build` (outputs to `dist/`)
- Deploy: `npm run deploy` (gh-pages to configured homepage)

**Run Single Test**
```powershell
npx vitest src/utils/__tests__/deduplicate.test.ts --run
```

## Architecture Overview

FinTracker is a personal finance management SPA built with React 19 + TypeScript + Vite. It supports importing transactions from CSV/JSON/MessagePack, deduplicating them, and visualizing data through multiple chart types. The app stores all data locally in the browser (via file system access APIs).

### High-Level Data Flow

1. **Upload** → CsvUploader parses CSV and creates Transaction objects
2. **Deduplication** → findDuplicates() checks against existing transactions; unresolved duplicates go to DuplicateResolver UI
3. **Filtering** → FilterContext global stat
```

</details>
