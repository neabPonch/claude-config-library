---
name: jasonlong__mater
source: https://github.com/jasonlong/mater/blob/86357f096e21610e37696ad581a6974e6b2adf3c/CLAUDE.md
repo: jasonlong/mater
kind: claude-md
stars: 583
last_pushed: 2026-04-14T15:00:59Z
license: mit
score: 8
domains: [desktop-app, electron]
tags: [architecture, process-communication, electron]
curated: 2026-06-16
curated_by: config-scout
---

# jasonlong/mater — claude-md

**Why it's worth keeping:** It explicitly details the main vs. renderer relationship and highlights non-obvious technical details like `globalThis.sharedObject` access which prevents hallucinated interaction methods.

**Summary:** Provides a concise breakdown of Electron's multi-process architecture and its communication patterns.

**Source credibility:** High; a well-regarded, highly starred macOS utility project.

**Recency:** Very current; updated within the last few months.

**Source:** [jasonlong/mater/CLAUDE.md](https://github.com/jasonlong/mater/blob/86357f096e21610e37696ad581a6974e6b2adf3c/CLAUDE.md) · 583★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Mater is a minimal Pomodoro timer menubar app built with Electron. It runs a 25-minute work timer followed by a 5-minute break, repeating until stopped.

## Commands

- `npm start` - Run the app in development mode
- `npm test` - Run all linters (JS + CSS) and e2e tests
- `npm run lint:js` - Run XO (ESLint-based) JavaScript linter
- `npm run lint:css` - Run Stylelint CSS linter
- `npm run bundle` - Bundle renderer.js (production, minified)
- `npm run bundle:dev` - Bundle renderer.js (dev, with sourcemaps)
- `npm run make` - Build installer for current platform (uses Electron Forge)
- `npm run make:mac` / `make:linux` / `make:win` - Build for specific platform

## Architecture

This is a standard Electron app with two processes:

- **main.js** - Main process: creates the menubar using the `menubar` package, handles tray icon and context menu (sound toggle, quit)
- **renderer.js** - Renderer process: manages timer logic using `tiny-timer`, handles UI state transitions (stopped/working/breaking), updates tray icons per minute
- **index.html** - Sing
```

</details>
