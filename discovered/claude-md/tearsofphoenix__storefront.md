---
name: tearsofphoenix__storefront
source: https://github.com/tearsofphoenix/storefront/blob/e020f42feb1fd49521498f9ff45a313a6cca2f02/CLAUDE.md
repo: tearsofphoenix/storefront
kind: claude-md
stars: 0
last_pushed: 2026-04-27T01:54:57Z
license: mit
score: 9
domains: [web-frontend, ecommerce, monorepo]
tags: [nextjs, payload-cms, medusa, monorepo, ecommerce]
curated: 2026-06-15
curated_by: config-scout
---

# tearsofphoenix/storefront — claude-md

**Why it's worth keeping:** Excellent breakdown of architectural flows (payment redirects, i18n-driven routing) and clear separation of commands by application context.

**Summary:** A comprehensive guide for a Next.js and Payload CMS monorepo that details specific business logic and integration patterns.

**Source credibility:** The repo has low social proof (0 stars), but the documentation density suggests a sophisticated real-world implementation.

**Recency:** Highly current, utilizing modern technologies like Next.js 15, Bun, and Payload 3.

**Source:** [tearsofphoenix/storefront/CLAUDE.md](https://github.com/tearsofphoenix/storefront/blob/e020f42feb1fd49521498f9ff45a313a6cca2f02/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Panda Commerce monorepo — a composable ecommerce platform with two independent apps:

- **`apps/storefront/`** — Customer-facing Medusa storefront (Next.js 15 + Bun)
- **`apps/payload-cms/`** — Headless CMS for landing/product pages (Payload 3 + pnpm)

The Medusa backend lives in a separate repo (`store-pandacat-ai`) and is already configured with payment modules for ECPay and PAYUni.

## Commands

### Storefront (`apps/storefront/` or root)

```bash
bun install                    # Install dependencies
bun run dev                    # Dev server on :8000 (turbopack)
bun run build                  # Production build
bun run start                  # Start production server on :8000
bun run lint                   # ESLint
```

### Payload CMS (`apps/payload-cms/`)

```bash
pnpm install                   # Install dependencies
pnpm dev                       # Dev server (generates import map first)
pnpm build                     # Production build
pnpm lint                      # ESLint
pnpm test:int                  # Unit tests (Vitest)
pnpm test:
```

</details>
