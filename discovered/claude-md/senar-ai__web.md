---
name: senar-ai__web
source: https://github.com/senar-ai/web/blob/42935480cbe8e20721ee5297e5d8a6bc176a6eb4/CLAUDE.md
repo: senar-ai/web
kind: claude-md
stars: 88
last_pushed: 2025-08-30T08:32:48Z
license: unknown
score: 7
domains: [web-frontend, fullstack]
tags: [remix, deno, prisma, tailwind]
curated: 2026-06-16
curated_by: config-scout
---

# senar-ai/web — claude-md

**Why it's worth keeping:** Crucially distinguishes between Node.js and Deno dependency management to prevent environment errors; provides specific data flow logic.

**Summary:** Provides clear command mappings and architectural guidance for a Remix application running on the Deno runtime.

**Source credibility:** Standard project documentation from a specialized web repository.

**Recency:** 

**Source:** [senar-ai/web/CLAUDE.md](https://github.com/senar-ai/web/blob/42935480cbe8e20721ee5297e5d8a6bc176a6eb4/CLAUDE.md) · 88★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Essential Commands

### Development

- `npm run dev` - Start development server with file watching
- `npm run build` - Build for production
- `npm start` - Run production build
- `npm run fetch` - Fetch database from external source (senarai-db)

### Code Quality

- `npm run format` - Format code using pkode
- `npm run lint` - Lint code using pkode
- `npm run test` - Run tests using pkode
- `npm run test:update` - Update test snapshots

### CSS

- `npm run generate:css` - Generate Tailwind CSS
- `npm run dev:css` - Generate CSS with watch mode

### Database (Prisma)

- `npx prisma generate` - Update TypeScript definitions
- `npx prisma db push` - Push schema changes to database
- `npx prisma studio` - Open Prisma Studio
- `npx prisma migrate dev --name <name>` - Generate migration
- `npx prisma migrate reset` - Reset migrations and run seed

### Deployment

- `npm run deploy` - Deploy to Deno Deploy

## Architecture Overview

This is a **Remix + Deno** application that serves as a learning resources directory ("Senarai"). Key architectural patterns:

### Tech Stac
```

</details>
