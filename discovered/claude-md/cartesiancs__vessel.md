---
name: cartesiancs__vessel
source: https://github.com/cartesiancs/vessel/blob/d7230fdf68f0be174891eb66cc7e40c45a5a9106/CLAUDE.md
repo: cartesiancs/vessel
kind: claude-md
stars: 326
last_pushed: 2026-05-31T15:01:07Z
license: apache-2.0
score: 9
domains: [backend-rust, web-frontend, desktop-app, systems-programming]
tags: [monorepo-mapping, architecture-patterns, mission-critical]
curated: 2026-06-16
curated_by: config-scout
---

# cartesiancs/vessel — claude-md

**Why it's worth keeping:** It excels at explaining high-level system patterns (state management/concurrency) alongside specific low-level coding constraints like deterministic execution rules.

**Summary:** Provides a comprehensive architectural map and mental model for a complex polyglot monorepo involving Rust, React, and Tauri.

**Source credibility:** High; comes from an active, specialized repo in the physical AI space.

**Recency:** Highly current, referencing bleeding-edge technologies like React 19 and Tailwind v4.

**Source:** [cartesiancs/vessel/CLAUDE.md](https://github.com/cartesiancs/vessel/blob/d7230fdf68f0be174891eb66cc7e40c45a5a9106/CLAUDE.md) · 326★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Guidance for Claude Code working in the Vessel repository.

## Project

Vessel is C2 (Command & Control) software for connecting, monitoring, and orchestrating physical sensors through a visual flow-based interface. Local-first, offline-first. Apache-2.0.

## Repository layout

Cargo + npm workspaces (monorepo).

- `apps/server` — Rust (axum, tokio) backend. SQLite via Diesel (`migrations/`, schema in `src/db/schema.rs`). MQTT broker (rumqttd) + client (rumqttc), WebRTC, RTP/RTSP via GStreamer, ONNX inference (ort/tract). Entry: `src/main.rs`. Routes wired in `src/routes.rs`, handlers under `src/handler/`. Flow engine in `src/flow/` (engine, manager, nodes). Built-in flow nodes live in `src/flow/nodes/`. The compiled server embeds the client `dist/` via `rust-embed`.
- `apps/client` — React 19 + Vite + TypeScript + Tailwind v4 + Radix + Zustand. FSD-ish layout: `app/`, `pages/`, `widgets/`, `features/`, `entities/`, `shared/`, plus `components/ui` (shadcn) and `hooks/`, `contexts/`, `lib/`. Routing in `src/App.tsx` (react-router v7).
- `apps/desktop` — Tauri v2 shell. The Tauri build runs `cargo build --release -p server` and bundles the server binary as a sidecar; fro
```

</details>
