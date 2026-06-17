---
name: Marco6-3__music
source: https://github.com/Marco6-3/music/blob/6c70b87cf5082f4c658790c4cd7b7afafc1ccf23/CLAUDE.md
repo: Marco6-3/music
kind: claude-md
stars: 0
last_pushed: 2026-06-12T15:24:52Z
license: unknown
score: 8
domains: [desktop-app, electron, backend-api]
tags: [architecture-mapping, regression-prevention, verification-steps]
curated: 2026-06-15
curated_by: config-scout
---

# Marco6-3/music — claude-md

**Why it's worth keeping:** It uses 'negative constraints' to prevent regressive patterns (like restoring old SQLite paths) and provides specific command flags for probing different system states.

**Summary:** Detailed architectural map that connects specific files to their functional responsibilities and includes a verification checklist.

**Source credibility:** Low popularity/star count, but the content reflects high-quality project organization from an individual developer.

**Recency:** Current; it explicitly references Claude Code and modern development workflows.

**Source:** [Marco6-3/music/CLAUDE.md](https://github.com/Marco6-3/music/blob/6c70b87cf5082f4c658790c4cd7b7afafc1ccf23/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file gives Claude Code repository-specific guidance for this project.

## Project Overview

`music` is a Windows desktop music player rebuilt with Electron, an Express 5 local backend, and a static frontend/PWA under `webroot/`.

The current backend runs locally and can be started with plain Node. Web/PWA mode should be deployed over HTTPS for iPhone Safari/Home Screen use. Do not reintroduce the old Electron Node wrapper or native SQLite dependency path.

## Commands

```powershell
npm start
npm run dev
npm run server
npm run web:start
npm test
npm run test:pwa
npm run probe:sources
npm run probe:backend
npm run qa:electron
npm run dist
npm run build
npm run pack
npm run installer
```

Fallback testing flags:

```powershell
npm run probe:sources -- --disable-gdstudio
npm run probe:sources -- --disable-unm
npm run probe:sources -- --disable-meting
npm run probe:sources -- --disable-lrclib
```

## Architecture

### Electron

- `src/main.js`: Electron main process, window lifecycle, splash screen, backend startup, version polling, window-state persistence, tray entry, cache-aware reload.
- `src/preload.js`: exposes safe renderer APIs through `contextBridge`.
- `src/
```

</details>
