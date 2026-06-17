---
name: jvillegasd__media-bridge
source: https://github.com/jvillegasd/media-bridge/blob/8eb58839d336ff3a0f85ea5292db2f276663e2d6/CLAUDE.md
repo: jvillegasd/media-bridge
kind: claude-md
stars: 4
last_pushed: 2026-03-07T09:32:28Z
license: mit
score: 9
domains: [browser-extensions, web-media, javascript]
tags: [architecture-mapping, constraints-documentation, edge-cases]
curated: 2026-06-15
curated_by: config-scout
---

# jvillegasd/media-bridge — claude-md

**Why it's worth keeping:** It goes beyond 'how to run' by documenting the 'mental model' of the system: edge cases (crash resilience), physical constraints (2GB limit), and specific failure modes (JSON serialization of ArrayBuffers). This allows an AI to reason about side effects across different execution contexts.

**Summary:** Provides a deep architectural blueprint for a multi-context Chrome Extension including service worker, offscreen document, and content script interactions. It explicitly documents system constraints like memory limits, concurrency requirements, and data serialization pitfalls.

**Source credibility:** Highly credible; a well-structured, specialized media tool with recent maintenance.

**Recency:** 

**Source:** [jvillegasd/media-bridge/CLAUDE.md](https://github.com/jvillegasd/media-bridge/blob/8eb58839d336ff3a0f85ea5292db2f276663e2d6/CLAUDE.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
# Development build with watch mode (rebuilds on file changes)
npm run dev

# Production build (minified, no sourcemaps)
npm run build

# TypeScript type checking only (no emit)
npm run type-check
```

There are no tests in this project. After building, load the `dist/` directory as an unpacked extension in Chrome (`chrome://extensions/` → Developer mode → Load unpacked).

## Output Size Limit

All HLS, M3U8, and DASH downloads are processed by the muxer running inside the browser. Output files are limited to approximately **2 GB** — files beyond this will exhaust browser memory during the merge stage.

## Cloud Upload

`src/core/cloud/` contains the full provider abstraction:

- `base-cloud-provider.ts` — abstract `BaseCloudProvider` with `id: CloudProvider` and `upload(blob, filename, onProgress?, signal?): Promise<string>`
- `google-auth.ts` — `GoogleAuth` static class; OAuth via `chrome.identity.launchWebAuthFlow()` with user-provided client ID (stored in `chrome.storage.local` under `google_client_id`). No `oauth2` manifest key needed.
- `go
```

</details>
