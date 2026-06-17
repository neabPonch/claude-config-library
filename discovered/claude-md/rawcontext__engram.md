---
name: rawcontext__engram
source: https://github.com/rawcontext/engram/blob/1553e53ff5b09eb55d22cd2b1e75bd6e9d90dc42/CLAUDE.md
repo: rawcontext/engram
kind: claude-md
stars: 6
last_pushed: 2026-01-05T20:10:48Z
license: agpl-3.0
score: 9
domains: [agents-ai, monorepo, backend]
tags: [bun, python, mcp, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# rawcontext/engram — claude-md

**Why it's worth keeping:** Uses highly effective 'Do vs Don't' comparison tables to enforce runtime APIs and provides specific file paths as architectural anchor points for the agent.

**Summary:** A high-density guide for a complex hybrid TypeScript/Python monorepo focused on AI memory infrastructure.

**Source credibility:** Low star count but demonstrates high-level engineering maturity through specialized documentation.

**Recency:** Highly current, utilizing modern runtimes like Bun and uv.

**Source:** [rawcontext/engram/CLAUDE.md](https://github.com/rawcontext/engram/blob/1553e53ff5b09eb55d22cd2b1e75bd6e9d90dc42/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Engram

Bitemporal, graph-backed intelligent agent memory system. Hybrid TypeScript/Python monorepo.

## Critical Commands

```bash
# TypeScript (bun workspaces)
bun install              # Install all workspaces
bun run infra:up         # Start all services (Observatory, Search, Tuner, DBs)
bun run infra:down       # Stop infrastructure
bun run dev              # Start all apps in dev mode
bun run build            # Build all apps/packages
bun run test             # Run Bun's native test runner
bun run typecheck        # TypeScript validation
bun run lint             # Biome linting
bun run format           # Biome formatting

# Python apps (uv)
cd apps/search && uv sync      # Install dependencies
cd apps/search && uv run pytest  # Run tests
cd apps/search && uv run ruff check src tests  # Lint
cd apps/search && uv run ruff format src tests  # Format
cd apps/search && uv run search  # Start service

cd apps/tuner && uv sync       # Install tuner dependencies
cd apps/tuner && uv run tuner  # Start tuner service

# OAuth verification
./scripts/verify-oauth-setup.sh  # Verify local OAuth configuration
```

## Local Development - OAuth Setup

**CRITICAL**: All services require OAuth
```

</details>
