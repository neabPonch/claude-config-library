---
name: evrendom__rudel
source: https://github.com/evrendom/rudel/blob/1f8f15aa9568229e26dbdf1d9495d7b3882361a9/CLAUDE.md
repo: evrendom/rudel
kind: claude-md
stars: 284
last_pushed: 2026-05-19T09:19:33Z
license: mit
score: 9
domains: [fullstack, monorepo, data-engineering]
tags: [bun, typescript, clickhouse, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# evrendom/rudel — claude-md

**Why it's worth keeping:** It provides explicit domain logic constraints—specifically for image/avatar handling—and clearly delineates between local Docker workflows and production-data dev modes to prevent environment errors.

**Summary:** A high-density technical overview of a Bun-based monorepo involving dual-database architecture (Postgres and ClickHouse).

**Source credibility:** High; the project demonstrates a professional, sophisticated architecture using modern tools like Bun and orpc.

**Recency:** Very current; uses contemporary stack components and development patterns.

**Source:** [evrendom/rudel/CLAUDE.md](https://github.com/evrendom/rudel/blob/1f8f15aa9568229e26dbdf1d9495d7b3882361a9/CLAUDE.md) · 284★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Rudel

A platform for ingesting, storing, and analyzing Claude Code / Codex session transcripts. Users authenticate via the web app, use the CLI to upload `.jsonl` session transcripts, which are stored in ClickHouse for analytics.

**Stack**: Bun, Turborepo, Biome, TypeScript
**Deployment**: Bun server + Postgres (Neon) + ClickHouse
**Domain**: `app.rudel.ai`

## Monorepo Structure

### Apps

| App | Package | Description |
|-----|---------|-------------|
| `apps/api` | `@rudel/api` | HTTP API server (Bun). Auth via `better-auth`, RPC via `@orpc/server`, session ingestion into ClickHouse. |
| `apps/cli` | `rudel` (npm) | CLI tool for authenticating and uploading Claude Code / Codex session transcripts. Commands: `login`, `logout`, `whoami`, `upload`. |
| `apps/web` | `@rudel/web` | React SPA (Vite + Tailwind + shadcn). Auth UI and CLI login portal. |

### Packages

| Package | Description |
|---------|-------------|
| `packages/api-routes` (`@rudel/api-routes`) | Shared RPC contract (`@orpc/contract` + Zod schemas). Single source of truth for the API interface. |
| `packages/ch-schema` (`@rudel/ch-schema`) | ClickHouse table schema (`rudel.claude_sessions`, `rudel.session_analyti
```

</details>
