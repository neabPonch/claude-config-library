---
name: ScopeCreep-zip__SpiritStream
source: https://github.com/ScopeCreep-zip/SpiritStream/blob/edaf1919d6d064cc3516a6ac8be99fdecd6e8feb/CLAUDE.md
repo: ScopeCreep-zip/SpiritStream
kind: claude-md
stars: 19
last_pushed: 2026-05-25T20:24:30Z
license: gpl-3.0
score: 9
domains: [fullstack, desktop-app, rust, react]
tags: [workspace-management, tech-stack-specs, architecture-driven]
curated: 2026-06-15
curated_by: config-scout
---

# ScopeCreep-zip/SpiritStream — claude-md

**Why it's worth keeping:** Provides explicit build commands for different workspaces (web vs desktop) and leverages specific version pinning (React 19, Tailwind v4). The pattern of referencing sub-files like `.claude/rules/coding-standards.md` is a professional way to manage large-scale project context.

**Summary:** A highly structured technical spec that bridges high-level architecture with low-level coding standards and environment configurations. It utilizes a modular context system via a dedicated .claude/ directory.

**Source credibility:** Active repository with recent updates and clear technical depth.

**Recency:** Extremely current; uses modern tech stacks like React 19 and Tailwind v4.

**Source:** [ScopeCreep-zip/SpiritStream/CLAUDE.md](https://github.com/ScopeCreep-zip/SpiritStream/blob/edaf1919d6d064cc3516a6ac8be99fdecd6e8feb/CLAUDE.md) · 19★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SpiritStream

Desktop streaming application with RTMP stream management, FFmpeg processing, and multi-output streaming with profile management.

**Repository**: https://github.com/ScopeCreep-zip/SpiritStream

## Architecture

Host server (Rust/Axum) + Client (React) — desktop via Tauri sidecar, also Docker and web browser access.

See `.claude/rules/architecture.md` for full details.

## Tech Stack

| Layer | Technology |
|-------|------------|
| Backend | Rust + Axum 0.7 |
| Frontend | React 19 + TypeScript 5.9 |
| Styling | Tailwind CSS v4 |
| Build | Vite 7 + Turbo |
| State | Zustand 5 |
| i18n | i18next (11 locales) |
| Desktop | Tauri 2.x (launcher only) |

## Build Commands

```bash
pnpm dev                  # All workspaces (Turbo)
pnpm dev:web              # Frontend only (localhost:5173)
pnpm dev:desktop          # Desktop app (Tauri + server sidecar)

pnpm build                # All workspaces (Turbo)
pnpm build:web            # Frontend only
pnpm build:desktop        # Desktop app with sidecar

pnpm typecheck            # TypeScript checking (Turbo)
cargo check --manifest-path server/Cargo.toml               # Server
cargo check --manifest-path apps/desktop/src-tauri/
```

</details>
