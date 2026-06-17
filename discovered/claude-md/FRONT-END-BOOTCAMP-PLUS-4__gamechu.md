---
name: FRONT-END-BOOTCAMP-PLUS-4__gamechu
source: https://github.com/FRONT-END-BOOTCAMP-PLUS-4/gamechu/blob/83f514cfcf9d8b4189cb184521927fdd68bdaf07/CLAUDE.md
repo: FRONT-END-BOOTCAMP-PLUS-4/gamechu
kind: claude-md
stars: 1
last_pushed: 2026-05-08T08:48:17Z
license: unknown
score: 9
domains: [web-frontend, backend-api, fullstack]
tags: [nextjs, clean-architecture, ddd, structured-docs]
curated: 2026-06-15
curated_by: config-scout
---

# FRONT-END-BOOTCAMP-PLUS-4/gamechu — claude-md

**Why it's worth keeping:** Uses a 'drill-down' documentation strategy (pointing to specific files like CACHING.md) to manage complexity without context bloat; includes vital architectural guardrails like singleton and instantiation rules.

**Summary:** A high-density configuration that acts as a central router to a granular, hierarchical system of project conventions.

**Source credibility:** Single star repo, likely a bootcamp or personal project, but demonstrates high engineering discipline.

**Recency:** Highly current, utilizing Next.js 15 and Prisma 6.

**Source:** [FRONT-END-BOOTCAMP-PLUS-4/gamechu/CLAUDE.md](https://github.com/FRONT-END-BOOTCAMP-PLUS-4/gamechu/blob/83f514cfcf9d8b4189cb184521927fdd68bdaf07/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## 겜추(GameChu)

Korean game recommendation and community platform live at gamechu.com

## Commands

```bash
npm run dev        # Start dev server with Turbopack
npm run build      # Production build
npm run start      # Run production server on port 3035
npx prisma migrate dev    # Run DB migrations
npx prisma generate       # Regenerate Prisma client after schema changes
```

```bash
npm test           # Run unit tests (Vitest, 126 tests)
npm run lint       # Run ESLint
npm run format     # Run Prettier
npm run test:e2e   # Run Playwright E2E tests
```

## Architecture

**Next.js 15 full-stack app** (App Router) using **Clean Architecture + DDD** in the backend layer.

## Tech Stack

- **Frontend**: Next.js 15 (App Router), React 19, TypeScript, TailwindCSS 3, Zustand 5, Framer Motion, Lexical (rich text editor)
- **Backend**: PostgreSQL, Prisma 6, Redis (ioredis), Socket.io 4, NextAuth.js v4, Zod 4
- **Testing**: Vitest 4, Playwright, Testing Library
- **Tooling**: ESLint, Prettier, Husky

## Git Workflow (overrides skill defaults)

- Whenever deals with git(include git, gh, and GitHub mcp), Read `docs/conventions/GIT_COLLABORATION.md`

## Conventions

Full code conventions: `doc
```

</details>
