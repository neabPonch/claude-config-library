---
name: codante-io__guias
source: https://github.com/codante-io/guias/blob/e9db0d74e176571950b0893b6be691165b2ee4cc/CLAUDE.md
repo: codante-io/guias
kind: claude-md
stars: 4
last_pushed: 2025-11-05T20:22:15Z
license: unknown
score: 8
domains: [web-frontend, monorepo]
tags: [astro, nextjs, pnpm, starlight]
curated: 2026-06-16
curated_by: config-scout
---

# codante-io/guias — claude-md

**Why it's worth keeping:** Outlines critical architectural constraints like specific base paths for guides and provides a step-by-step 'Adding New Guide' workflow to ensure consistency.

**Summary:** Defines a pnpm monorepo containing multiple Astro/Starlight sites and a Next.js landing page.

**Source credibility:** High-quality documentation from an organized technical learning repository (Codante.io).

**Recency:** Current, utilizing modern frameworks like Next.js 14 and Astro.

**Source:** [codante-io/guias/CLAUDE.md](https://github.com/codante-io/guias/blob/e9db0d74e176571950b0893b6be691165b2ee4cc/CLAUDE.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

pnpm monorepo for Codante.io guides. Each guide is a separate app built with Starlight (Astro framework). Home app is Next.js 14.

## Architecture

- **Monorepo structure**: Root manages workspaces in `apps/*`
- **Home app** (`apps/home`): Next.js 14 landing page, lists all guides
- **Guide apps**: Astro + Starlight sites for documentation/tutorials
  - Each has own `base` path in `astro.config.mjs` (e.g., `/next-auth/`)
  - Content in `src/content/docs/` with auto-generated sidebars
  - Tailwind CSS via `@astrojs/tailwind` with `applyBaseStyles: false`

## Commands

### Development
```bash
# Install deps (from root)
pnpm i

# Run specific guide locally
cd apps/[guide-name]
pnpm run dev
```

### Build/Deploy
```bash
# Build all apps (from root)
pnpm -r run build

# Build specific app
cd apps/[guide-name]
pnpm run build  # or 'astro check --minimumSeverity warning && astro build' for guides with checks
```

### Guides structure
Most Astro guides:
- `dev/start`: dev server
- `build`: build (some include `astro check --minimumSeverity warning`)
- `p
```

</details>
