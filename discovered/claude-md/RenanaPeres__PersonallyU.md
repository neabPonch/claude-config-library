---
name: RenanaPeres__PersonallyU
source: https://github.com/RenanaPeres/PersonallyU/blob/8cd9be22424ca900e83c151867256c1fa8dcb725/CLAUDE.md
repo: RenanaPeres/PersonallyU
kind: claude-md
stars: 0
last_pushed: 2026-06-07T11:52:21Z
license: unknown
score: 8
domains: [web-frontend, e-commerce]
tags: [shopify, liquid, state-management, ecommerce]
curated: 2026-06-15
curated_by: config-scout
---

# RenanaPeres/PersonallyU — claude-md

**Why it's worth keeping:** It maps complex business logic—specifically the flow of quiz data through localStorage to UI changes—which prevents the AI from breaking core functionality. It also explicitly warns against looking for build steps/npm, which is vital for non-standard workflows.

**Summary:** Defines a Shopify Liquid theme driven by a custom personality-based personalization system.

**Source credibility:** Low visibility repository (0 stars), but documentation density indicates a real-world application.

**Recency:** Current; includes modern Shopify CLI and dev workflow instructions.

**Source:** [RenanaPeres/PersonallyU/CLAUDE.md](https://github.com/RenanaPeres/PersonallyU/blob/8cd9be22424ca900e83c151867256c1fa8dcb725/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

PersonallyU is a customized Shopify Liquid theme (based on Craft v15.2.0) for a personality-based merchandise store. Users take a quiz that determines their personality type, and the site routes them to personalized product pages.

## Development Workflow

This is a **Shopify Liquid theme** — there is no build step, no package.json, and no npm. There is no local dev server.

**To develop:**
- Edit files directly in this repo
- Use [Shopify CLI](https://shopify.dev/docs/themes/tools/cli) to preview locally: `shopify theme dev`
- Push to GitHub; sync to Shopify admin via the GitHub integration

**To deploy:**
- Changes on `main` sync to the Shopify store via the GitHub ↔ Shopify admin connection

## Architecture

### Tech Stack
- **Shopify Liquid** — server-side templating for all pages
- **Vanilla JavaScript (ES6+)** + **jQuery 3.6** — loaded globally via `layout/theme.liquid`
- **Plain CSS** — component-scoped files in `assets/`
- No React, Vue, or build pipeline

### Key Directories
- `layout/` — master templates (`theme.liquid` is the root HTML
```

</details>
