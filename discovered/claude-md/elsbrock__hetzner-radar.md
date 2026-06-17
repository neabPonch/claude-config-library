---
name: elsbrock__hetzner-radar
source: https://github.com/elsbrock/hetzner-radar/blob/4cc8640591c3a6a8c2b52a75a0066b184c21f987/CLAUDE.md
repo: elsbrock/hetzner-radar
kind: claude-md
stars: 336
last_pushed: 2026-06-15T04:46:06Z
license: agpl-3.0
score: 8
domains: [web-frontend, fullstack, cloud-infrastructure]
tags: [sveltekit, typescript, cloudflare, duckdb]
curated: 2026-06-15
curated_by: config-scout
---

# elsbrock/hetzner-radar — claude-md

**Why it's worth keeping:** It explicitly defines high-value syntax patterns like Svelte 5 runes and clarifies the dual-database architecture (DuckDB vs D1) to prevent AI architectural errors.

**Summary:** Provides a technical blueprint for a SvelteKit/Cloudflare application, clearly distinguishing between client-side and server-side data layers.

**Source credibility:** High; active maintenance and significant community interest indicated by star count.

**Recency:** Highly current, specifically accounting for modern shifts like Svelte 5 syntax.

**Source:** [elsbrock/hetzner-radar/CLAUDE.md](https://github.com/elsbrock/hetzner-radar/blob/4cc8640591c3a6a8c2b52a75a0066b184c21f987/CLAUDE.md) · 336★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Hetzner Server Radar Project Context

## Project Overview

Hetzner Server Radar is a web application that tracks prices of Hetzner's Dedicated Server Auction over time. It helps customers identify the best configurations and prices by providing advanced filtering, pricing history, and target price alerts.

## Technology Stack

- **Frontend**: SvelteKit 5 with TypeScript
- **Styling**: Tailwind CSS with Flowbite components
- **Database**: DuckDB (client-side) and Cloudflare D1 (backend)
- **Deployment**: Cloudflare Pages with Workers
- **Data Processing**: Python 3 with Poetry for package management
- **Testing**: Playwright for E2E tests, Vitest for unit tests

## Key Commands

```bash
# Development
npm run dev          # Start development server
npm run build        # Build for production
npm run preview      # Preview production build
npm run check        # Run svelte-check
npm run lint         # Run prettier and eslint
npm run format       # Format code with prettier
npm run test         # Run tests

# Python/Data Processing
poetry shell         # Enter Python environment
python scripts/import.py data static/sb.duckdb  # Import data
```

## Project Structure

- `/src/routes/`
```

</details>
