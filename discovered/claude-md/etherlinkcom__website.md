---
name: etherlinkcom__website
source: https://github.com/etherlinkcom/website/blob/55cd13cfe28c64de94c961e16fa7be83cebd0bc4/CLAUDE.md
repo: etherlinkcom/website
kind: claude-md
stars: 14
last_pushed: 2026-05-18T17:22:00Z
license: other
score: 9
domains: [web-frontend, cms-integration]
tags: [nextjs, strapi, typescript, tailwind]
curated: 2026-06-15
curated_by: config-scout
---

# etherlinkcom/website — claude-md

**Why it's worth keeping:** Explicitly documents architectural constraints (e.g., no API routes, unoptimized images) and 'gotchas' like hardcoded sections to prevent AI hallucinations.

**Summary:** A comprehensive technical specification for a Next.js static export site integrated with Strapi CMS.

**Source credibility:** Active real-world project maintained within the last month.

**Recency:** Highly current, utilizing modern Next.js App Router and Strapi v5 patterns.

**Source:** [etherlinkcom/website/CLAUDE.md](https://github.com/etherlinkcom/website/blob/55cd13cfe28c64de94c961e16fa7be83cebd0bc4/CLAUDE.md) · 14★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Etherlink.com is the marketing and ecosystem directory website for the Etherlink blockchain. It is a **statically exported Next.js 13 site** (App Router) using **Strapi v5 (GraphQL)** as the headless CMS for project listings and tags. Built with TypeScript, Tailwind CSS, and Flowbite React.

## Commands

```bash
bun install --no-save   # Install dependencies (without modifying lockfile)
bun dev                  # Dev server at localhost:3000
npm run build            # Static export to out/
npm start                # Serve the static out/ directory
npm run lint             # ESLint check
npm run lint:fix         # ESLint auto-fix
npm run format           # Prettier format
```

Pre-commit hook runs `bunx lint-staged` which applies `eslint --fix` to staged `.js/.ts/.tsx` files.

## Architecture

### Static Export

`next.config.js` sets `output: 'export'` with `distDir: 'out'`. All pages are pre-rendered at build time. There are **no API routes**. Images are unoptimized (required for static export).

### Strapi CMS

Data is fetched from Strapi v5 via
```

</details>
