---
name: yinMrsir__chunyu-cms-v2
source: https://github.com/yinMrsir/chunyu-cms-v2/blob/9ff8be01e885504e40f2f45a59b6beb225d52ed6/CLAUDE.md
repo: yinMrsir/chunyu-cms-v2
kind: claude-md
stars: 64
last_pushed: 2026-03-19T03:22:27Z
license: mit
score: 9
domains: [web-frontend, backend-api, monorepo]
tags: [nuxt, drizzle-orm, cms, monorepo]
curated: 2026-06-14
curated_by: config-scout
---

# yinMrsir/chunyu-cms-v2 — claude-md

**Why it's worth keeping:** The 'Common Development Tasks' section provides perfect SOPs for an AI to follow when adding new features, and the directory-specific command lists are essential for monorepos.

**Summary:** A highly detailed guide for a Nuxt-based video CMS that clarifies monorepo navigation and database schema management.

**Source credibility:** Moderate popularity (64 stars) with recent maintenance activity.

**Recency:** Very current; uses modern stacks like Nuxt 3, Drizzle ORM, and pnpm.

**Source:** [yinMrsir/chunyu-cms-v2/CLAUDE.md](https://github.com/yinMrsir/chunyu-cms-v2/blob/9ff8be01e885504e40f2f45a59b6beb225d52ed6/CLAUDE.md) · 64★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

淳渔CMS V2 (Chunyu CMS V2) is a modern video content management system designed for rapid development of video websites. It's a complete overhaul from V1, replacing NestJS with Nuxt 3 for both frontend and backend functionality in a monorepo structure.

## Technology Stack

- **Frontend**: Vue 3 + Element Plus + TypeScript (admin), Nuxt 3 + UnoCSS (web)
- **Backend**: Nuxt 3 with Nitro server engine
- **Database**: MySQL 8.0+ with Drizzle ORM
- **Cache**: Redis for session storage and caching
- **Package Manager**: pnpm (8.9.2+)
- **Node.js**: 18.16.0+ (managed by Volta)

## Development Commands

### Web Application (chunyu-cms-web/)

```bash
cd chunyu-cms-web
pnpm dev              # Start development server on localhost:3000
pnpm dev:pro          # Start with production environment config
pnpm build            # Build for production
pnpm preview          # Preview production build
pnpm lint             # Run ESLint and Prettier checks
pnpm lintfix          # Auto-fix linting issues
pnpm generate         # Generate Drizzle ORM migration files
pnpm
```

</details>
