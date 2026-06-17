---
name: artsmc__sprint-ui
source: https://github.com/artsmc/sprint-ui/blob/6cc8c120fac13945f961a5ff6a4a057a838517f1/CLAUDE.md
repo: artsmc/sprint-ui
kind: claude-md
stars: 2
last_pushed: 2026-03-21T04:05:01Z
license: mit
score: 8
domains: [web-frontend, fullstack, devops]
tags: [nextjs, docker, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# artsmc/sprint-ui — claude-md

**Why it's worth keeping:** Includes critical Docker networking details and path aliases that prevent the AI from making incorrect connectivity or import assumptions.

**Summary:** Provides essential technical context for a full-stack Next.js and PocketBase application including architectural flows and dev commands.

**Source credibility:** Low star count, but demonstrates organized development via 'memory-bank' references.

**Recency:** Extremely current, leveraging Next.js 16 and React 19.

**Source:** [artsmc/sprint-ui/CLAUDE.md](https://github.com/artsmc/sprint-ui/blob/6cc8c120fac13945f961a5ff6a4a057a838517f1/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Sprint UI is a biweekly design challenge platform where designers receive prompts, submit designs, and vote/provide anonymous feedback on each other's work. Built with Next.js 16 (App Router), React 19, PocketBase backend, and Docker.

## Commands

```bash
npm run dev      # Start dev server (port 3000)
npm run build    # Production build
npm run start    # Run production server
npm run lint     # ESLint check

# Docker (recommended for full stack)
docker-compose up --build  # Next.js (3000) + PocketBase (8090)
```

PocketBase admin: http://localhost:8090/_/

## Architecture

```
Client Browser
    ↓
Next.js App Router (app/)
    ↓
Library Layer (lib/pocketbase.ts, env.ts)
    ↓
PocketBase Backend (Auth, SQLite DB, Realtime, Files)
```

**Key files:**
- `env.ts` - T3 Env with Zod validation for type-safe environment variables
- `lib/pocketbase.ts` - Singleton PocketBase client instance
- `app/layout.tsx` - Root layout with global styles
- `app/page.tsx` - Home page

**Path alias:** `@/` maps to project root (e.g., `import { env } from '@/env'`)
```

</details>
