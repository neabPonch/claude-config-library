---
name: HEIGE-PCloud__DoIt
source: https://github.com/HEIGE-PCloud/DoIt/blob/e4151744f910209dfe1e81eaa3c9b715e230e6f2/CLAUDE.md
repo: HEIGE-PCloud/DoIt
kind: claude-md
stars: 931
last_pushed: 2026-06-11T10:03:54Z
license: mit
score: 9
domains: [web-frontend, static-site-generator]
tags: [hugo, tailwind-v4, documentation]
curated: 2026-06-15
curated_by: config-scout
---

# HEIGE-PCloud/DoIt — claude-md

**Why it's worth keeping:** Crucial specific detail regarding the 'tw:' Tailwind prefix and detailed explanation of how templates/partials interact prevents common errors.

**Summary:** Provides a clear mental model of the Hugo theme architecture and essential development commands.

**Source credibility:** High; a popular, highly-starred open-source project with recent activity.

**Recency:** Current; mentions modern technologies like Tailwind v4 and Hugo extended requirements.

**Source:** [HEIGE-PCloud/DoIt/CLAUDE.md](https://github.com/HEIGE-PCloud/DoIt/blob/e4151744f910209dfe1e81eaa3c9b715e230e6f2/CLAUDE.md) · 931★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

DoIt is a Hugo theme — a template package for the Hugo static site generator. It is not a standalone web app. The `exampleSite/` directory contains a demo Hugo site that uses the theme.

## Commands

```bash
# Development (Hugo server + Tailwind CSS watch, concurrent)
npm run dev

# Production build
npm run build

# Build with draft content
npm run build:preview

# Hugo dev server only (no Tailwind)
npm run server

# Tailwind CSS only (watch mode)
npm run server:tailwind

# Format code
npm run format

# W3C HTML validation (requires Docker)
npm run validate

# Visual regression tests (requires Hugo running)
npx playwright test
```

Hugo requires the **extended** version 0.146.0 or higher. Nix users: `flake.nix` provides the full environment automatically via direnv.

## Architecture

### Directory Layout

- `layouts/` — Hugo HTML templates (the core of the theme)
  - `_partials/` — reusable partials included by other templates
  - `_shortcodes/` — 25+ custom Hugo shortcodes for rich content
  - `_markup/` — render hooks for Markdown elements (lin
```

</details>
