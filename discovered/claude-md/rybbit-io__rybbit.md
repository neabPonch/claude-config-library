---
name: rybbit-io__rybbit
source: https://github.com/rybbit-io/rybbit/blob/35f6e768d70f2263d935568b545109f8458b5fef/CLAUDE.md
repo: rybbit-io/rybbit
kind: claude-md
stars: 12293
last_pushed: 2026-06-12T21:48:15Z
license: agpl-3.0
score: 8
domains: [web-frontend, backend-api, fullstack]
tags: [monorepo, typescript, design-system]
curated: 2026-06-15
curated_by: config-scout
---

# rybbit-io/rybbit — claude-md

**Why it's worth keeping:** It utilizes high-level 'negative constraints' (e.g., never run migrations) and links to strategic design/product docs to prevent architectural drift.

**Summary:** Provides precise command execution paths for a monorepo and integrates deep product context via external documentation files.

**Source credibility:** High; repository has 12k+ stars and active maintenance.

**Recency:** Current; specifically references Claude Code capabilities.

**Source:** [rybbit-io/rybbit/CLAUDE.md](https://github.com/rybbit-io/rybbit/blob/35f6e768d70f2263d935568b545109f8458b5fef/CLAUDE.md) · 12293★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

- Client: `cd client && npm run dev` (NextJS with Turbopack on port 3002)
- Server: `cd server && npm run dev` (TypeScript backend)
- Lint: `cd client && npm run lint` or `cd server && npm run build`
- TypeCheck: `cd client && tsc --noEmit` or `cd server && tsc`
- Database: `cd server && npm run db:push` (update DB schema)

## Code Conventions

- TypeScript with strict typing throughout both client and server
- Client: React functional components with minimal useEffect and inline functions
- Frontend: Next.js, Tailwind CSS, Shadcn UI, Tanstack Query, Zustand, Luxon, Nivo, react-hook-form
- Backend: Fastify, Drizzle ORM (Postgres), ClickHouse, Zod
- Error handling: Use try/catch blocks with specific error types
- Naming: camelCase for variables/functions, PascalCase for components/types
- Imports: Group by external, then internal (alphabetical within groups)
- File organization: Related functionality in same directory
- Dark mode is default theme
- Never run any database migration scripts

## Design Context

- `PRODUCT.md` (repo root) — strategic design c
```

</details>
