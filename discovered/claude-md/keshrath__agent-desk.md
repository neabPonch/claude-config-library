---
name: keshrath__agent-desk
source: https://github.com/keshrath/agent-desk/blob/42dddfb7a14fd6ba936c45abe1c54f2012e16a2e/CLAUDE.md
repo: keshrath/agent-desk
kind: claude-md
stars: 1
last_pushed: 2026-04-15T21:57:39Z
license: mit
score: 9
domains: [monorepo, electron-app, systems-architecture]
tags: [architectural-boundaries, ipc-contract, environment-purity]
curated: 2026-06-14
curated_by: config-scout
---

# keshrath/agent-desk — claude-md

**Why it's worth keeping:** It provides explicit 'no-go' rules to prevent environment leakage (e.g., no Electron imports in core) and includes a deterministic step-by-step protocol for extending the IPC system.

**Summary:** Defines strict architectural boundaries and a formal communication contract for an Electron/Web monorepo.

**Source credibility:** Low star count, but the high level of architectural specificity suggests a sophisticated real-world tool.

**Recency:** Highly current; last pushed 2 months ago.

**Source:** [keshrath/agent-desk/CLAUDE.md](https://github.com/keshrath/agent-desk/blob/42dddfb7a14fd6ba936c45abe1c54f2012e16a2e/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# agent-desk

Dual-target AI agent control center: Electron desktop app AND web/PWA, sharing one transport-agnostic core.

## Overview

agent-desk runs as either:
- **Desktop**: Electron shell wrapping `@agent-desk/core` via IPC bridge.
- **Server + Web/PWA**: Node Express+ws server driving the same core over WebSocket, mobile PWA as a read-only (v1) client.

The renderer (`@agent-desk/ui`) is vanilla JS with zero Electron dependencies — it talks to whatever transport `window.agentDesk` is wired to.

## Workspace layout

```
packages/
  core/       @agent-desk/core     — transport-agnostic Node, no Electron
  desktop/    @agent-desk/desktop  — Electron main + preload, IPC bridge to core
  ui/         @agent-desk/ui       — vanilla JS renderer, zero Electron deps
  server/     @agent-desk/server   — Node Express+ws, single-user token auth, WS → core
  pwa/        @agent-desk/pwa      — thin mobile-optimized read-only entry over server
docs/         vitepress site (docs:dev / docs:build / docs:preview)
```

### `@agent-desk/core` public exports

From `packages/core/src/index.ts`:

- `TerminalManager` (+ `ManagedTerminal`, `TerminalClient`, `HistoryEntry`)
- `startMonitoring`, `stopMo
```

</details>
