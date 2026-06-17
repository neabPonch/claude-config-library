---
name: agenda__agenda
source: https://github.com/agenda/agenda/blob/b9c47688d2803e9627a4ef8a07466434cc1f7cae/CLAUDE.md
repo: agenda/agenda
kind: claude-md
stars: 9675
last_pushed: 2026-06-12T10:06:47Z
license: other
score: 9
domains: [backend, node.js, distributed-systems]
tags: [monorepo, architecture, system-design]
curated: 2026-06-16
curated_by: config-scout
---

# agenda/agenda — claude-md

**Why it's worth keeping:** Uses ASCII-based architecture maps and highlights critical implementation 'gotchas' like specific DB indexes and required error handlers.

**Summary:** Provides deep architectural context, including monorepo command patterns and component relationships.

**Source credibility:** High; based on a highly-starred, actively maintained Node.js library.

**Recency:** Current; reflects the latest repository state and monorepo structure.

**Source:** [agenda/agenda/CLAUDE.md](https://github.com/agenda/agenda/blob/b9c47688d2803e9627a4ef8a07466434cc1f7cae/CLAUDE.md) · 9675★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Agenda is a lightweight job scheduling library for Node.js with pluggable storage backends. It's a TypeScript rewrite of agenda.js with full typing and improvements for distributed job processing.

This is a pnpm monorepo with the following packages:
- `packages/agenda` - Core scheduler (published as "agenda" on npm)
- `packages/mongo-backend` - MongoDB backend (published as "@agendajs/mongo-backend" on npm)
- `packages/postgres-backend` - PostgreSQL backend (published as "@agendajs/postgres-backend" on npm)
- `packages/redis-backend` - Redis backend (published as "@agendajs/redis-backend" on npm)
- `packages/agendash` - Placeholder for dashboard integration

## Common Commands

```bash
# Build all packages
pnpm build

# Testing (runs all package tests)
pnpm test

# Run agenda package tests directly
pnpm --filter agenda test

# Run single test file
pnpm --filter agenda exec vitest run test/job.test.ts

# Run tests matching a pattern
pnpm --filter agenda exec vitest run --grep "pattern"

# Debug with agenda logging
DEBUG=agenda:**,-agenda:internal
```

</details>
