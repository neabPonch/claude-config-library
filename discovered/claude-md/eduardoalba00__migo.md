---
name: eduardoalba00__migo
source: https://github.com/eduardoalba00/migo/blob/ea7221c45eb3ccca6dd443051b1ee56670cf8a7f/CLAUDE.md
repo: eduardoalba00/migo
kind: claude-md
stars: 2
last_pushed: 2026-03-02T04:42:01Z
license: agpl-3.0
score: 9
domains: [desktop-app, real-time-media, monorepo, fullstack]
tags: [electron, fastify, pnpm-monorepo, livekit]
curated: 2026-06-16
curated_by: config-scout
---

# eduardoalba00/migo — claude-md

**Why it's worth keeping:** It includes crucial technical 'gotchas' (like why LiveKit runs natively vs Docker) and detailed directory maps that help an AI navigate complex package dependencies.

**Summary:** Provides high-signal architectural overviews, monorepo orchestration details, and specific deployment/infrastructure configurations.

**Source credibility:** Small open-source project with high-quality, professionally structured documentation.

**Recency:** 

**Source:** [eduardoalba00/migo/CLAUDE.md](https://github.com/eduardoalba00/migo/blob/ea7221c45eb3ccca6dd443051b1ee56670cf8a7f/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build & Dev Commands

```bash
# Install dependencies
pnpm install

# Dev (Postgres via Docker + LiveKit native + Fastify — all in one command)
pnpm dev                 # Starts everything, Ctrl+C stops all
pnpm dev:client          # Electron + Vite React app (separate terminal)
pnpm dev:client2         # Second client instance (MIGO_INSTANCE=2)

# Production (self-hosted)
pnpm prod:setup              # Interactive setup: generates .env.prod with secrets, starts services
pnpm prod:start              # Starts Postgres + server + Watchtower (Docker) + LiveKit (native)
pnpm prod:stop               # Stops all prod services

# Production builds
pnpm build:server        # tsc → packages/server/dist/
pnpm build:client        # electron-vite build

# Database (Drizzle ORM + PostgreSQL)
pnpm db:generate         # Generate migration files from schema changes
pnpm db:migrate          # Apply migrations (tsx src/db/migrate.ts)

# Native addon (Windows only)
cd packages/client && npx node-gyp rebuild   # Compile WASAPI audio capture addon
node src/native/test-capture.cjs
```

</details>
