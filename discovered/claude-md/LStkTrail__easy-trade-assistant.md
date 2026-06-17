---
name: LStkTrail__easy-trade-assistant
source: https://github.com/LStkTrail/easy-trade-assistant/blob/6a1ee184d7d81739d1fb485dafdff119e56a49cc/CLAUDE.md
repo: LStkTrail/easy-trade-assistant
kind: claude-md
stars: 0
last_pushed: 2026-03-18T15:31:18Z
license: mit
score: 7
domains: [desktop-app, rust, web-frontend]
tags: [tauri, vue, rust, fullstack]
curated: 2026-06-16
curated_by: config-scout
---

# LStkTrail/easy-trade-assistant — claude-md

**Why it's worth keeping:** The 'Key Files to Reference' section provides high-value entry points for pattern discovery, while the architecture section explains how frontend and backend layers interface via Serde.

**Summary:** Defines a full-stack Tauri/Rust desktop environment, covering build commands and IPC communication patterns.

**Source credibility:** Low (0 stars); likely a personal/small-scale project.

**Recency:** 

**Source:** [LStkTrail/easy-trade-assistant/CLAUDE.md](https://github.com/LStkTrail/easy-trade-assistant/blob/6a1ee184d7d81739d1fb485dafdff119e56a49cc/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Technology Stack

- **Frontend**: Vue 3 + TypeScript + Vite
- **Backend**: Rust (via Tauri 2)
- **Package manager**: pnpm

## Common Commands

### Development
```bash
pnpm tauri dev          # Start full dev environment (Vite + Tauri)
pnpm dev                 # Start only Vite dev server (port 1420)
```

### Build
```bash
pnpm tauri build         # Build full desktop application
pnpm build               # Build frontend only (type check + Vite build)
pnpm preview             # Preview built frontend
```

### Type Checking
```bash
pnpm build               # Runs vue-tsc --noEmit for type checking
```

### Testing & Linting
- No test framework currently configured
- No linting configured

## High-Level Architecture

This is a Tauri 2 desktop application with a standard two-layer architecture:

1. **Frontend Layer**: Vue 3 single-page application running in a system webview
   - Entry point: `src/main.ts`
   - Main component: `src/App.vue`
   - Built with Vite to `dist/` directory

2. **Backend Layer**: Rust binary that manages the system window
   - Entry point: `sr
```

</details>
