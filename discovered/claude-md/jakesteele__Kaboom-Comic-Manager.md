---
name: jakesteele__Kaboom-Comic-Manager
source: https://github.com/jakesteele/Kaboom-Comic-Manager/blob/58e24b5fb0fcd29585bac7d0fecdf008662c3872/CLAUDE.md
repo: jakesteele/Kaboom-Comic-Manager
kind: claude-md
stars: 0
last_pushed: 2026-03-25T05:02:10Z
license: mit
score: 9
domains: [backend-api, web-frontend, monorepo]
tags: [nuxt, fastify, sqlite, docker, pnpm, opds]
curated: 2026-06-15
curated_by: config-scout
---

# jakesteele/Kaboom-Comic-Manager — claude-md

**Why it's worth keeping:** The 'Key Design Decisions' section is invaluable; it prevents the AI from making classic errors like treating synchronous SQLite queries as async or misconfiguring static file routing.

**Summary:** Provides deep architectural context for a Fastify/Nuxt monorepo, including specific implementation constraints and technical gotchas.

**Source credibility:** A niche personal project with high-density, professional-grade documentation.

**Recency:** 

**Source:** [jakesteele/Kaboom-Comic-Manager/CLAUDE.md](https://github.com/jakesteele/Kaboom-Comic-Manager/blob/58e24b5fb0fcd29585bac7d0fecdf008662c3872/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Kaboom Comic Manager

## Project Overview
Kaboom is a self-hosted OPDS 1.2 server for serving CBZ, CBR, and ePub comic/manga/book files to readers like Panels (iPad). It includes a web UI for library management built with Nuxt 3.

## Architecture

### Monorepo (pnpm workspaces)
```
shared/    — TypeScript types, constants, regex patterns (@opds/shared)
server/    — Fastify 5 backend with SQLite (better-sqlite3 via Drizzle ORM) (@opds/server)
web/       — Nuxt 3 SPA frontend with @nuxt/ui (@opds/web)
docker/    — Dockerfile and docker-compose.yml
```

### Key Design Decisions
- **SPA mode (ssr: false)** — Nuxt generates static HTML/JS, served by Fastify in Docker
- **Content negotiation at `/`** — Browsers get the SPA (text/html), OPDS clients get XML catalog
- **Synchronous DB** — better-sqlite3 is sync; use `.get()`, `.all()`, `.run()` (no await needed)
- **tsx in production** — TypeScript runs directly via globally-installed tsx, no build step for server
- **`nuxt generate` (not `nuxt build`)** — Required for static SPA output with index.html in `.output/public/`
- **Relative API URLs** — SPA uses empty `API_BASE` in production (same-origin); dev uses `http://localhost:3000`

#
```

</details>
