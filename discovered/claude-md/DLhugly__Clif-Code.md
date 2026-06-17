---
name: DLhugly__Clif-Code
source: https://github.com/DLhugly/Clif-Code/blob/1857d740d454d28de2019382e511934ec3e83bdc/CLAUDE.md
repo: DLhugly/Clif-Code
kind: claude-md
stars: 14
last_pushed: 2026-04-26T16:22:30Z
license: other
score: 7
domains: [cli-tools, desktop-apps, rust, web-frontend, monorepo]
tags: [tauri, rust, solidjs, monorepo, tui]
curated: 2026-06-14
curated_by: config-scout
---

# DLhugly/Clif-Code — claude-md

**Why it's worth keeping:** The 'Conventions' section provides actionable syntax guardrails (e.g., SolidJS attribute naming) that prevent common AI mistakes. The explicit mapping of file purposes across different sub-projects is highly effective for navigating monorepos.

**Summary:** Provides an organized map of a dual-product monorepo containing a Tauri-based desktop IDE and a Rust TUI agent. It bridges high-level project structure with specific implementation constraints.

**Source credibility:** A niche, active open-source project with recent commits and a clear technical profile.

**Recency:** Very current; utilizes modern tech stacks like Tauri 2 and Tailwind CSS 4.

**Source:** [DLhugly/Clif-Code/CLAUDE.md](https://github.com/DLhugly/Clif-Code/blob/1857d740d454d28de2019382e511934ec3e83bdc/CLAUDE.md) · 14★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Clif-Code Monorepo

Two products in one repo:

## ClifPad (`clif-pad-ide/`)
Desktop AI-native code editor — Tauri 2 + SolidJS + Monaco Editor.

**Tech**: Tauri 2 (Rust), SolidJS, TypeScript, Monaco, Tailwind CSS 4, Vite 6
**AI**: OpenRouter API, Ollama, Claude Code CLI

```
cd clif-pad-ide && npm install && npm run tauri dev
```

### Layout
- `clif-pad-ide/src/` — SolidJS frontend (components, stores, types)
- `clif-pad-ide/src-tauri/` — Rust backend (commands, services, state)
- `clif-pad-ide/www/` — Landing page (clifcode.io, deployed via Vercel)
- `clif-pad-ide/scripts/` — Version bump script

### Conventions
- SolidJS: `class=` not `className=`, stores in `src/stores/`
- Tauri commands in `src-tauri/src/commands/`, IPC wrappers in `src/lib/tauri.ts`
- AI streaming via Tauri events ("ai_stream", "claude-code-output")

## ClifCode (`clif-code-tui/`)
TUI terminal agent — Rust, API-only (no local model inference).

```
cd clif-code-tui && cargo run --release
```

### Layout
- `clif-code-tui/src/main.rs` — CLI, TUI loop, agent orchestration
- `clif-code-tui/src/backend.rs` — API backend (OpenRouter, OpenAI, Ollama)
- `clif-code-tui/src/tools.rs` — Tool definitions and execution
-
```

</details>
