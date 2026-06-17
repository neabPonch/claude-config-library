---
name: ychisbest__The-Farmer-Was-Replaced
source: https://github.com/ychisbest/The-Farmer-Was-Replaced/blob/93eee4c867caf51c89ff9218866e6ee233d73b8f/CLAUDE.md
repo: ychisbest/The-Farmer-Was-Replaced
kind: claude-md
stars: 18
last_pushed: 2026-05-27T03:10:50Z
license: unknown
score: 8
domains: [web-frontend, i18n]
tags: [astro, tailwind-css, multilingual]
curated: 2026-06-15
curated_by: config-scout
---

# ychisbest/The-Farmer-Was-Replaced — claude-md

**Why it's worth keeping:** It clearly maps complex i18n URL patterns to the file structure and component hierarchy. The inclusion of 'Development Workflow' steps provides a template for projects with non-standard startup sequences.

**Summary:** This config provides deep context for a multilingual Astro.js site, specifically detailing the dynamic routing used for i18n.

**Source credibility:** Small project (18 stars) but contains highly structured, high-quality documentation.

**Recency:** Very current; references modern versions like Astro 5 and Tailwind CSS 4.

**Source:** [ychisbest/The-Farmer-Was-Replaced/CLAUDE.md](https://github.com/ychisbest/The-Farmer-Was-Replaced/blob/93eee4c867caf51c89ff9218866e6ee233d73b8f/CLAUDE.md) · 18★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a multilingual website for "The Farmer Was Replaced" - an educational programming game. The site is built with Astro.js and Tailwind CSS, featuring internationalization (i18n) support for English and Chinese languages.

## Development Commands

### Essential Commands
- `npm run dev` - Start development server with hot reload
- `npm run build` - Build production static site
- `npm run preview` - Preview production build locally
- `npm run astro` - Run Astro CLI commands directly

### Development Workflow
1. Run `npm run dev` to start development server
2. The site supports both English (default) and Chinese languages
3. Default locale (English) doesn't have URL prefix, Chinese uses `/zh` prefix
4. All pages are in the `src/pages/[...lang]/` directory structure

## Architecture & Structure

### Core Technologies
- **Astro 5** - Static site generator with islands architecture
- **Tailwind CSS 4** - Utility-first CSS framework (via Vite plugin)
- **TypeScript** - Type-safe development
- **MDX** - Enhanced markdown with React components

### I
```

</details>
