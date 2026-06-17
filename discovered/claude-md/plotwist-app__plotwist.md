---
name: plotwist-app__plotwist
source: https://github.com/plotwist-app/plotwist/blob/de8cdeb9b732ff822966f0ff75d94e30d02d2c9e/CLAUDE.md
repo: plotwist-app/plotwist
kind: claude-md
stars: 439
last_pushed: 2026-04-24T21:43:59Z
license: other
score: 9
domains: [web-frontend, backend-api, mobile-ios, monorepo]
tags: [DDD, SwiftUI, Next.js, Monorepo, DesignTokens]
curated: 2026-06-15
curated_by: config-scout
---

# plotwist-app/plotwist — claude-md

**Why it's worth keeping:** The 'Do not' lists and explicit code templates prevent common LLM hallucinations; the architecture breakdown provides immediate context for folder navigation.

**Summary:** A comprehensive guide for a full-stack monorepo that includes strict architectural constraints and specific command sets.

**Source credibility:** High quality, well-maintained repository with significant stars.

**Recency:** Extremely current, utilizing modern frameworks like Next.js 16 and Fastify 5.

**Source:** [plotwist-app/plotwist/CLAUDE.md](https://github.com/plotwist-app/plotwist/blob/de8cdeb9b732ff822966f0ff75d94e30d02d2c9e/CLAUDE.md) · 439★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Plotwist is a media management app (movies, series, anime) with three main apps in a pnpm/Turbo monorepo:
- `apps/web` — Next.js 16 web app
- `apps/backend` — Fastify 5 REST API
- `apps/ios` — Native SwiftUI iOS app

## Commands

### Root (all apps via Turbo)
```bash
pnpm run dev          # Start all dev servers
pnpm run build        # Build all apps
pnpm run test         # Run all tests
pnpm run biome:check  # Lint + format check
pnpm run biome:format # Format code
```

### Web (`apps/web`)
```bash
pnpm run dev          # Next.js dev server
pnpm run build        # Production build
pnpm run test         # Vitest unit tests
pnpm run typecheck    # TypeScript type check
pnpm run generate:api # Regenerate API types from backend OpenAPI spec (Orval)
```

### Backend (`apps/backend`)
```bash
make run              # Start dev server (tsx watch)
make test             # Run Vitest tests
make lint             # Biome lint
make build            # Production build (tsup)
make compose-up       # Start Docker (Postgres, Redis, LocalStack S3)
make compose-down
```

</details>
