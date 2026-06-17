---
name: kevin7lou__blog
source: https://github.com/kevin7lou/blog/blob/0ac26b830bcbc0f5b7df7ad54dd32b3c80031e10/CLAUDE.md
repo: kevin7lou/blog
kind: claude-md
stars: 2
last_pushed: 2026-04-13T16:00:53Z
license: mit
score: 7
domains: [web-frontend, static-site-generator]
tags: [astro, markdown, i18n]
curated: 2026-06-15
curated_by: config-scout
---

# kevin7lou/blog — claude-md

**Why it's worth keeping:** Includes critical 'gotchas' like the i18n limitation for client-side scripts and explicit instructions for content creation tasks.

**Summary:** A highly specific guide for an Astro 5 static site including tech stack, directory structure, and deployment workflows.

**Source credibility:** Low star count personal repository; value derived from documentation specificity rather than social proof.

**Recency:** Very current, utilizing modern technologies like Astro 5 and Tailwind CSS v4.

**Source:** [kevin7lou/blog/CLAUDE.md](https://github.com/kevin7lou/blog/blob/0ac26b830bcbc0f5b7df7ad54dd32b3c80031e10/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal blog ("Memory Palace") powered by Astro 5 + AstroPaper v5 theme, deployed to GitHub Pages and Vercel.

- **Site URL:** https://kevin7lou.github.io/blog
- **Author:** Kevin Lou
- **Language:** zh-CN (Chinese content, Chinese UI)

## Commands

```bash
npm run dev       # Local dev server (http://localhost:4321)
npm run build     # Generate static site to ./dist
npm run preview   # Preview built site locally
```

Create a new post: add a `.md` file in `src/data/blog/` with required front matter (`title`, `pubDatetime`, `description`, `tags`).

## Architecture

### Tech Stack

Astro 5 + Tailwind CSS v4 + TypeScript + Shiki + Pagefind. Zero framework dependencies (no React/Svelte/Vue).

### Key Directories

- `src/data/blog/` — Blog posts (Markdown with Zod-validated front matter)
- `src/components/` — Astro components (Header, Footer, TOC, Reward, etc.)
- `src/layouts/` — Page layouts (Layout.astro base, PostDetails.astro for posts)
- `src/i18n/` — Chinese UI translations (zh.ts + t() helper)
- `src/pages/` — File-based routing
- `src/config
```

</details>
