---
name: besscroft__PicImpact
source: https://github.com/besscroft/PicImpact/blob/21bd6e6729e234db8c5796406f779c0566bf0dd7/CLAUDE.md
repo: besscroft/PicImpact
kind: claude-md
stars: 1282
last_pushed: 2026-06-12T19:55:11Z
license: mit
score: 9
domains: [web-frontend, backend-api, fullstack]
tags: [nextjs, hono, api-specification, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# besscroft/PicImpact — claude-md

**Why it's worth keeping:** The incredibly specific API response envelope requirements, code snippet examples for helpers, and clear separation of DB read/write operations prevent AI from breaking the established pattern.

**Summary:** A highly detailed guide that provides strict architectural constraints and API design specifications for a fullstack Next.js/Hono application.

**Source credibility:** Strong; comes from a high-star (1282), actively maintained photography portfolio project.

**Recency:** Highly current; utilizes very recent technologies like Next.js 16 and Tailwind CSS v4.

**Source:** [besscroft/PicImpact/CLAUDE.md](https://github.com/besscroft/PicImpact/blob/21bd6e6729e234db8c5796406f779c0566bf0dd7/CLAUDE.md) · 1282★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# PicImpact

Self-deployable photography portfolio website built with Next.js 16 + Hono.js + PostgreSQL.

## Quick Reference

```bash
# Development
pnpm run dev:server          # Start dev server
pnpm run dev:turbopack       # Dev with Turbopack

# Build
pnpm run build               # Production build
pnpm run build:vercel        # Vercel deployment build
pnpm run build:node          # Node.js deployment build

# Database
pnpm run prisma:generate     # Generate Prisma client
pnpm run prisma:dev          # Run dev migrations
pnpm run prisma:deploy       # Deploy migrations
pnpm run prisma:seed         # Seed initial data

# Linting
pnpm run lint                # ESLint check
pnpm run lint:fix            # Auto-fix lint issues
```

## Tech Stack

- **Framework:** Next.js 16 + React 19 + TypeScript (strict mode)
- **Backend API:** Hono.js (routes in `hono/`)
- **Database:** PostgreSQL + Prisma ORM (`prisma/schema.prisma`)
- **Auth:** better-auth (email/password, TOTP 2FA, WebAuthn Passkeys)
- **Styling:** Tailwind CSS v4 + Radix UI + shadcn/ui
- **State:** Zustand + SWR
- **i18n:** next-intl (zh, en, ja, zh-TW)
- **Storage:** AWS S3 / Cloudflare R2 / Open List API

## Project Structur
```

</details>
