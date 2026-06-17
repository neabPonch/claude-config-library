---
name: codeErrorSleep__dbpaw
source: https://github.com/codeErrorSleep/dbpaw/blob/e59ad9fc2a4e68364d7778a059371e35738081a2/CLAUDE.md
repo: codeErrorSleep/dbpaw
kind: claude-md
stars: 245
last_pushed: 2026-06-15T09:48:47Z
license: apache-2.0
score: 8
domains: [fullstack, rust-tauri, database-client]
tags: [tauri, rust, react, developer-experience]
curated: 2026-06-16
curated_by: config-scout
---

# codeErrorSleep/dbpaw — claude-md

**Why it's worth keeping:** The 'Critical Rules' section enforces type synchronization and specific dev workflows, while the reference to an 'Immunity System' (AGENTS.md) is an elite pattern for preventing recurring agent errors.

**Summary:** Provides a structured mental model and high-stakes constraints for a full-stack Rust/Tauri application.

**Source credibility:** A well-maintained open-source database client with significant community interest (245 stars).

**Recency:** Current; utilizes modern tooling like Tauri v2 and Bun.

**Source:** [codeErrorSleep/dbpaw/CLAUDE.md](https://github.com/codeErrorSleep/dbpaw/blob/e59ad9fc2a4e68364d7778a059371e35738081a2/CLAUDE.md) · 245★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# DbPaw

Cross-platform database client (Tauri v2, React, Rust). Supports PostgreSQL, MySQL, MariaDB, TiDB, SQLite, SQL Server, ClickHouse, DuckDB.

## Quick Start
- `bun dev:mock` — Frontend-only dev (recommended for UI work)
- `bun tauri dev` — Full Tauri app with Rust backend
- `bun run test:smoke` — Quick validation (typecheck + lint + unit tests)
- `bun run test:all` — Full test suite

## Documentation Index
- **Architecture** → `docs/architecture.md` (frontend/backend structure, patterns, build system, i18n)
- **Commands** → `docs/commands.md` (all dev/test/lint commands)
- **Testing** → `docs/testing.md` (3-layer test strategy and coverage)
- **New Database Driver** → `docs/add-new-db.md` (step-by-step checklist)
- **Immunity System** → `AGENTS.md` (every line = a past agent failure, prevents repeat mistakes)
- **Design** → `docs/design.md`

## Critical Rules
- After modifying Rust code, always run `cargo check` (not just TypeScript compilation)
- New database drivers must be registered in `src-tauri/src/db/drivers/mod.rs` enum
- Tauri command parameter changes must sync `src/services/api.ts` type definitions
- Integration tests require Docker; use `IT_REUSE_LOCAL_DB=1` to s
```

</details>
