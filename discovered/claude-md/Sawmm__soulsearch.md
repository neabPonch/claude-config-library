---
name: Sawmm__soulsearch
source: https://github.com/Sawmm/soulsearch/blob/c1c1b52939a5fd096d84fbc8b0f8620012894d48/CLAUDE.md
repo: Sawmm/soulsearch
kind: claude-md
stars: 7
last_pushed: 2026-03-26T15:49:17Z
license: unknown
score: 9
domains: [cli-tools, audio-processing]
tags: [tui, typescript, ink, ffmpeg]
curated: 2026-06-15
curated_by: config-scout
---

# Sawmm/soulsearch — claude-md

**Why it's worth keeping:** It documents high-level business logic (like the FFT spectral analysis) that would be difficult to infer from code alone, preventing AI from breaking subtle technical implementations.

**Summary:** Provides deep architectural context for a TUI, including component hierarchy, focus systems, and a complex audio processing pipeline.

**Source credibility:** Small-scale project with 7 stars; documentation quality suggests a highly detail-oriented developer.

**Recency:** Highly relevant for current TypeScript/Node.js development workflows.

**Source:** [Sawmm/soulsearch/CLAUDE.md](https://github.com/Sawmm/soulsearch/blob/c1c1b52939a5fd096d84fbc8b0f8620012894d48/CLAUDE.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
npm run build       # TypeScript compile (tsc) → dist/
npm start           # Run compiled app: node dist/index.js
npm test            # Run tests with Vitest
npm run test:ci     # Type check + test (CI)
```

To run a single test file:
```bash
npx vitest run test/converter.test.ts
```

After `npm link`, the app is available as the global `soulsearch` CLI command.

## Architecture

**SoulSearch** is a Terminal UI (TUI) for the Soulseek P2P network, built with React + [Ink](https://github.com/vadimdemedes/ink) and TypeScript (ES modules). No backend server — it connects directly to Soulseek peers via `slsk-client`.

### Data Flow

```
src/index.tsx          Entry point — renders <App /> via Ink
src/App.tsx            Root component: connection, state, keyboard routing
  ├── src/api.ts       Soulseek + Discogs API, config loading, download streams
  ├── src/hooks/
  │   ├── useSearch.ts       Real-time search results + file stats
  │   ├── useDownloads.ts    Download lifecycle: queue → download → convert → organize
  │   └── useWishlistDaemon  Backgr
```

</details>
