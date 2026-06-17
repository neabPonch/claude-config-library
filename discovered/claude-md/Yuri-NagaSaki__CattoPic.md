---
name: Yuri-NagaSaki__CattoPic
source: https://github.com/Yuri-NagaSaki/CattoPic/blob/6ddd01758ae8c7f5020931fef4c068ece20e3abd/CLAUDE.md
repo: Yuri-NagaSaki/CattoPic
kind: claude-md
stars: 348
last_pushed: 2026-06-04T21:45:06Z
license: gpl-3.0
score: 8
domains: [fullstack, edge-computing, image-processing]
tags: [nextjs, cloudflare-workers, hono, r2, serverless]
curated: 2026-06-15
curated_by: config-scout
---

# Yuri-NagaSaki/CattoPic — claude-md

**Why it's worth keeping:** Includes critical business logic like R2 image path structures and mandatory changelog maintenance rules that prevent AI from deviating from project standards.

**Summary:** Defines the full-stack architecture for a Next.js and Cloudflare Worker project, including specific storage paths and environment mappings.

**Source credibility:** Solid mid-sized repo (348 stars) with active recent maintenance.

**Recency:** Highly current, utilizing modern patterns like Next.js App Router and Cloudflare Workers/Hono.

**Source:** [Yuri-NagaSaki/CattoPic/CLAUDE.md](https://github.com/Yuri-NagaSaki/CattoPic/blob/6ddd01758ae8c7f5020931fef4c068ece20e3abd/CLAUDE.md) · 348★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

CattoPic is an image hosting service with a Next.js frontend (deployed on Vercel) and a Cloudflare Worker backend (Hono framework) using R2 for storage and D1 for metadata.

**Important: This project uses pnpm as the package manager. Do not use npm or yarn.**

## Commands

### Frontend (Next.js)
```bash
pnpm dev          # Start dev server at localhost:3000
pnpm build        # Build for production
pnpm lint         # Run ESLint
```

### Worker (Cloudflare)
```bash
cd worker
pnpm dev          # Start local worker at localhost:8787
pnpm deploy       # Deploy to Cloudflare
pnpm wrangler d1 execute CattoPic-D1 --remote --file=schema.sql  # Init DB schema
```

## Architecture

```
├── app/                    # Next.js 16 frontend (App Router)
│   ├── components/         # React components
│   ├── hooks/              # Custom React hooks
│   ├── utils/              # Frontend utilities
│   └── manage/             # Admin management page
│
└── worker/                 # Cloudflare Worker backend
    └── src/
        ├── index.ts        # Hono router, rou
```

</details>
