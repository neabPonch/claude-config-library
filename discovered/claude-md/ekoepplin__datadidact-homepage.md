---
name: ekoepplin__datadidact-homepage
source: https://github.com/ekoepplin/datadidact-homepage/blob/ce3829b915d03f8bfde87ce96cf32026c3ec943e/CLAUDE.MD
repo: ekoepplin/datadidact-homepage
kind: claude-md
stars: 0
last_pushed: 2026-03-31T05:48:48Z
license: other
score: 8
domains: [web-frontend, static-site]
tags: [astro, tailwind, documentation, content-management]
curated: 2026-06-15
curated_by: config-scout
---

# ekoepplin/datadidact-homepage — claude-md

**Why it's worth keeping:** The 'Common Tasks' section provides actionable templates for repetitive actions, while the directory table prevents navigation errors by defining clear intent for each folder.

**Summary:** Provides a comprehensive blueprint for an Astro-based static site, covering specific commands, file mappings, and content schemas.

**Source credibility:** Low star count, but technical depth suggests a high-quality personal project.

**Recency:** Highly current, featuring bleeding-edge tech like Astro 5 and Tailwind 4.

**Source:** [ekoepplin/datadidact-homepage/CLAUDE.MD](https://github.com/ekoepplin/datadidact-homepage/blob/ce3829b915d03f8bfde87ce96cf32026c3ec943e/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## COMMANDS

### Development & Build
- Start local development server: `npm run dev`
- Build production site: `npm run build`
- Validate and build (with TypeScript check): `npm run build:check`
- Preview build locally: `npm run preview`

### Linting & Formatting
- Run linter: `npm run lint`
- Fix lint issues: `npm run lint:fix`
- Format code: `npm run format`
- Check code: `npm run check`
- Fix formatting issues: `npm run check:fix`

### Git Workflow
- Commit message convention: Conventional Commits via `cz`
- Run linter before commit in git hook: `biome check --write src`

## PROJECT ARCHITECTURE

### Tech Stack
- **Astro 5.x** - Static site generator with island architecture (React components inside static HTML)
- **TailwindCSS 4.x** - Utility-first CSS framework via @tailwindcss/vite plugin
- **React 19.x** - Used for interactive components via @astrojs/react
- **MDX** - Markdown + JSX support for blog posts
- **TypeScript 5.x** - Full type safety with ESLint/Biome integration

### Project Structure (src/)

| Directory | Purpose |
|-----------|---------|
| `conten
```

</details>
