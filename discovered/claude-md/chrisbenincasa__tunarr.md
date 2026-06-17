---
name: chrisbenincasa__tunarr
source: https://github.com/chrisbenincasa/tunarr/blob/412dc4662db3e2ce1779676c3ff367426708a47f/CLAUDE.md
repo: chrisbenincasa/tunarr
kind: claude-md
stars: 2352
last_pushed: 2026-06-12T01:34:38Z
license: zlib
score: 9
domains: [monorepo, backend-api, web-frontend]
tags: [typescript, pnpm, dependency-injection, fastify]
curated: 2026-06-15
curated_by: config-scout
---

# chrisbenincasa/tunarr — claude-md

**Why it's worth keeping:** It uses highly effective 'negative constraints' to prevent common runtime errors and provides explicit guidance on navigating the project's dependency injection system.

**Summary:** Acts as a comprehensive technical blueprint for a complex TypeScript monorepo, detailing architectural patterns and specific coding constraints.

**Source credibility:** High; repository has 2.3k+ stars and is actively maintained within the last month.

**Recency:** Extremely current, utilizing Node 22 and pnpm v10.

**Source:** [chrisbenincasa/tunarr/CLAUDE.md](https://github.com/chrisbenincasa/tunarr/blob/412dc4662db3e2ce1779676c3ff367426708a47f/CLAUDE.md) · 2352★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Tunarr is a live TV channel creation platform that allows users to create custom TV channels using media from local files or remote media servers such as Plex, Jellyfin, or Emby servers. It's a TypeScript monorepo using pnpm workspaces and Turbo for task running.

## Repository Structure

This is a monorepo with four main packages:

- **server** (`@tunarr/server`): Node.js backend (Fastify server, SQLite database)
- **web** (`@tunarr/web`): React frontend (Vite + Material-UI)
- **types** (`@tunarr/types`): Shared TypeScript types and Zod schemas
- **shared** (`@tunarr/shared`): Utility functions shared between server and web

## Code Style

- Never cast types using `as any`
- Never use inline `import()` type annotations — use top-level `import type` statements instead
- All edits must comply with the project's ESLint rules. Run `pnpm lint-changed` to verify before considering work complete
- **Nullability checks**: For values typed `T | undefined` (not `T | null`), always use `!== undefined` — never `!= null`. The loose equality `!= null` catches
```

</details>
