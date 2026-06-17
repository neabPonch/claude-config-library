---
name: itsdestin__youcoded
source: https://github.com/itsdestin/youcoded/blob/ad765e03293879e232cd82ea1b0271948f84f7f0/CLAUDE.md
repo: itsdestin/youcoded
kind: claude-md
stars: 6
last_pushed: 2026-06-14T19:46:00Z
license: other
score: 8
domains: [cross-platform, mobile-android, desktop-electron]
tags: [architecture, ipc-protocols, invariants]
curated: 2026-06-15
curated_by: config-scout
---

# itsdestin/youcoded — claude-md

**Why it's worth keeping:** Explicitly defines 'architectural invariants' and strict IPC surface requirements to prevent breaking platform parity between desktop and mobile builds.

**Summary:** Provides high-level architecture and protocol rules for a cross-platform Electron/Android ecosystem sharing a React UI.

**Source credibility:** Low star count, but the high technical density suggests a sophisticated engineering project.

**Recency:** Very recent; actively maintained within the last month.

**Source:** [itsdestin/youcoded/CLAUDE.md](https://github.com/itsdestin/youcoded/blob/ad765e03293879e232cd82ea1b0271948f84f7f0/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# YouCoded

This repo contains the YouCoded app — two platforms side by side:

- `desktop/` — Electron + React desktop app. See `desktop/CLAUDE.md` for architecture.
- `app/` — Android Kotlin app. See `.claude/rules/android-runtime.md` (auto-loaded for `app/**` edits) and `docs/android-runtime.md` in the `youcoded-dev` workspace scaffold for runtime constraints.

**The React UI is shared.** Android's WebView loads the same React bundle built from `desktop/src/renderer/` via `scripts/build-web-ui.sh`. The `app/build.gradle.kts` `bundleWebUi` task auto-runs the script before every APK build with input/output tracking, so a stale or missing bundle can no longer ship a blank-WebView APK. Run the script manually only when iterating outside Gradle.

**Android's terminal is also rendered by the shared React UI.** As of Tier 2, xterm.js running in the WebView is the sole Android terminal renderer — the native Termux `TerminalView` Compose block was removed. The vendored `terminal-emulator-vendored/` module owns the PTY + emulator and exposes raw bytes via the `pty:raw-bytes` WebSocket push event (base64-encoded); the WebView's xterm is display-only on touch (typing flows through the React
```

</details>
