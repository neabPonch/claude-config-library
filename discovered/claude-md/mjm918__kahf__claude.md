---
name: mjm918__kahf__claude
source: https://github.com/mjm918/kahf/blob/549e42c73d8ba6f22f47885f13dcc4996cab8940/.claude/claude.md
repo: mjm918/kahf
kind: claude-md
stars: 5
last_pushed: 2026-03-09T15:06:11Z
license: unknown
score: 9
domains: [full-stack, rust, angular, devops]
tags: [prescriptive, testing-heavy, ui-driven, high-density]
curated: 2026-06-15
curated_by: config-scout
---

# mjm918/kahf — claude-md

**Why it's worth keeping:** The 'Hard Rules' approach uses zero-tolerance constraints for code style (e.g., mandatory documentation blocks) and prevents AI hallucination by mapping UI components to a specific library. It also defines exactly what constitutes 'done' through a mandatory verification protocol involving execution and visual testing.

**Summary:** A high-rigor configuration that enforces strict architectural boundaries, coding styles, and defensive UX patterns for a full-stack Rust/Angular application. It mandates specific verification protocols using MCP tools like Playwright and dbhub.

**Source credibility:** Highly credible; reflects a professional-grade, complex engineering project with significant star count.

**Recency:** Very current; references modern versions of Angular (19), Rust, and Bun.

**Source:** [mjm918/kahf/.claude/claude.md](https://github.com/mjm918/kahf/blob/549e42c73d8ba6f22f47885f13dcc4996cab8940/.claude/claude.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# KahfLane — Claude Code Configuration

## Project Overview

KahfLane is a Huly-equivalent project management platform. Rust modular monolith backend (axum, sqlx, yrs CRDT) + Angular 19 + Syncfusion EJ2 frontend. Azure Portal-style UI. bun as the ONLY frontend runtime/package manager. Event-sourced data model with PostgreSQL 17 + TimescaleDB. Self-hosted via Docker Compose.

See `.claude/docs/plan/` for full architecture documents:
- `ARCHITECTURE_DESIGN.md` — Decisions, schema, crate structure, API design
- `IMPLEMENTATION_PLAN.md` — Phases, dependencies, project structure
- `MICROSERVICES_ARCHITECTURE.md` — Huly reference architecture (what we're replacing)
- `PLUGIN_SYSTEM.md` — Huly plugin system reference
- `SERVICES_ARCHITECTURE.md` — Huly services reference
- `UI_ARCHITECTURE.md` — Huly UI layout and navigation reference

## Running the Project

Run `./scripts/dev.sh` to start both backend and frontend. It kills existing instances on ports 3000/4200, starts the backend (`cargo run --bin kahf`), then the frontend (`bun run start`). Ctrl+C stops both.

## Hard Rules — Non-Negotiable

### Architecture
- EVERY module MUST be designed as an abstraction with traits/interfaces. No
```

</details>
