---
name: elirantutia__vibeyard
source: https://github.com/elirantutia/vibeyard/blob/14830f5a666f887d3bc2a898f73217fc444320ef/CLAUDE.md
repo: elirantutia/vibeyard
kind: claude-md
stars: 1221
last_pushed: 2026-06-04T12:04:37Z
license: mit
score: 9
domains: [electron, desktop-app, cli-tools, security]
tags: [electron, architecture, testing-patterns]
curated: 2026-06-14
curated_by: config-scout
---

# elirantutia/vibeyard — claude-md

**Why it's worth keeping:** The 'Architecture' section explicitly defines process boundaries (Main/Preload/Renderer) and the 'Testing' section provides specific implementation details for state cleanup between tests.

**Summary:** Provides deep architectural context for a multi-process Electron application, including build scripts and testing patterns. It details complex logic regarding CLI provider systems and security/profile isolation.

**Source credibility:** High; highly starred project with very recent activity.

**Recency:** Extremely current, updated within the last month.

**Source:** [elirantutia/vibeyard/CLAUDE.md](https://github.com/elirantutia/vibeyard/blob/14830f5a666f887d3bc2a898f73217fc444320ef/CLAUDE.md) · 1221★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

A terminal-centric IDE desktop app built on Electron that wraps CLI tool sessions. Users manage projects and sessions, each backed by a PTY running a CLI tool (currently Claude Code, with an abstraction layer for future providers like Copilot CLI and Gemini CLI), rendered via xterm.js.

## Build & Run

```bash
npm run build    # Compile all three targets (main, preload, renderer) + copy assets
npm start        # Build then launch Electron app (alias: npm run dev)
```

No hot reload — changes require rebuild + app restart.

Requires Node v24 (see `.nvmrc`). No lint tooling is configured.

Cross-platform: builds and runs on macOS, Linux, and Windows. Release artifacts (via electron-builder) include `.dmg`/`.zip` (mac), `.deb`/`.AppImage` (linux), and NSIS installer + portable `.exe` (win). CI covers all three platforms.

## Testing

```bash
npm test             # Run all tests once
npm run test:watch   # Watch mode (re-runs on file changes)
npm run test:coverage # Run with coverage report (terminal + HTML)
```

Uses **Vitest** with v8 coverage. Tests a
```

</details>
