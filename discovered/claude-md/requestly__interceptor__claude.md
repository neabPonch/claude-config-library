---
name: requestly__interceptor__claude
source: https://github.com/requestly/interceptor/blob/ca9aad0f6334595cb822ee2a3a066bd81ad9acb1/app/claude.md
repo: requestly/interceptor
kind: claude-md
stars: 16
last_pushed: 2026-06-13T07:58:51Z
license: other
score: 9
domains: [web-frontend, desktop-app, architecture]
tags: [react, state-management, multi-platform]
curated: 2026-06-15
curated_by: config-scout
---

# requestly/interceptor — claude-md

**Why it's worth keeping:** It explicitly defines the distinction between global (Redux) and local (Zustand) state management and enforces a strict backend integration layer to facilitate storage abstraction.

**Summary:** An architectural blueprint for a complex multi-platform React app spanning web, desktop, and extension environments.

**Source credibility:** High; part of an active open-source tool with recent maintenance.

**Recency:** 

**Source:** [requestly/interceptor/app/claude.md](https://github.com/requestly/interceptor/blob/ca9aad0f6334595cb822ee2a3a066bd81ad9acb1/app/claude.md) · 16★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
This is a React app that contains the UI code for Requestly. The same codebase runs in three different contexts:
- **Web browser** at https://app.requestly.io
- **Desktop app** (loaded inside Electron from `../../requestly-desktop-app`)
- **Browser extension** popup/options pages

The app adapts its behavior based on the environment using `window.RQ.MODE` and `window.RQ.DESKTOP`.

---

# Multi-Platform Support

The app detects its runtime environment and adapts:
- **Web mode**: Full web app experience
- **Desktop mode**: Enhanced with proxy control, file system access via IPC to desktop main/background processes
- **Extension mode**: Limited UI, communicates with extension background script

Communication bridges:
- **Desktop**: `window.RQ.DESKTOP` (IPC functions exposed via preload script)
- **Extension**: `chrome.runtime.sendMessage` / custom events

---

# Code Organization

## Primary Structure: Feature-Based

The **`features/`** directory is the main organizational unit. Each feature is a self-contained module:
- `apiClient/` - REST API client (Postman-like)
- `rules/` - Rule creation and management
- `mocks/` - Mock server
- `sessionBook/` - Session recording
- `settings/` -
```

</details>
