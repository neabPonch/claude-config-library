---
name: Tokisaki-Galaxy__sc-shop-frontend
source: https://github.com/Tokisaki-Galaxy/sc-shop-frontend/blob/77ab6ff8ace2c4e6f799d53efa6b87c14a01b534/CLAUDE.md
repo: Tokisaki-Galaxy/sc-shop-frontend
kind: claude-md
stars: 0
last_pushed: 2026-04-30T11:28:47Z
license: mit
score: 9
domains: [web-frontend, e-commerce, ai-agents]
tags: [nextjs-15, medusa-v2, architectural-patterns, agentic-workflow]
curated: 2026-06-15
curated_by: config-scout
---

# Tokisaki-Galaxy/sc-shop-frontend — claude-md

**Why it's worth keeping:** The 'Key Conventions' section provides explicit rules on SDK usage, cache tags, and data handling to prevent common developer errors. It also leverages a high-maturity pattern by directing Claude to load specific local agent skills.

**Summary:** A highly sophisticated guide that defines technical constraints, architectural patterns, and domain-driven organization. It uniquely integrates instructions for loading custom AI agent skills.

**Source credibility:** High-quality documentation for a specialized Medusa V2/Next.js 15 stack.

**Recency:** Extremely current, referencing Next.js 15 and modern e-commerce patterns.

**Source:** [Tokisaki-Galaxy/sc-shop-frontend/CLAUDE.md](https://github.com/Tokisaki-Galaxy/sc-shop-frontend/blob/77ab6ff8ace2c4e6f799d53efa6b87c14a01b534/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Medusa Next.js Starter Storefront — a production ecommerce storefront built with Next.js 15 (App Router) + Medusa V2 headless commerce backend. Based on the official Medusa Next.js Starter Template, customized for tokisaki's shop.

## Commands

```bash
pnpm dev              # Start dev server (Turbopack, port 8000)
pnpm build            # Production build
pnpm start            # Production server (port 8000)
pnpm lint             # ESLint
pnpm analyze          # Bundle analysis (ANALYZE=true build)
```

The storefront runs on port 8000 and expects a Medusa backend on port 9000 (configured via `MEDUSA_BACKEND_URL`).

## Environment Variables

Required: `MEDUSA_BACKEND_URL`, `NEXT_PUBLIC_MEDUSA_PUBLISHABLE_KEY`, `NEXT_PUBLIC_BASE_URL`, `NEXT_PUBLIC_DEFAULT_REGION`

Optional: `NEXT_PUBLIC_STRIPE_KEY`, `NEXT_PUBLIC_MEDUSA_PAYMENTS_PUBLISHABLE_KEY`, `NEXT_PUBLIC_MICROSOFT_CLARITY_ID`, `NEXT_PUBLIC_TURNSTILE_SITE_KEY`, `NEXT_PUBLIC_FILE_S3_URL`, `REVALIDATE_SECRET`

See `.env.template` for the full list.

## Architecture

### Routing: Country-Code Pref
```

</details>
