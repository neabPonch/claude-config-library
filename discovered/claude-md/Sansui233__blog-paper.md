---
name: Sansui233__blog-paper
source: https://github.com/Sansui233/blog-paper/blob/b76b9b6dc2fdb572db43d8131c96cad859fe6754/CLAUDE.md
repo: Sansui233/blog-paper
kind: claude-md
stars: 17
last_pushed: 2026-06-07T13:12:03Z
license: unknown
score: 8
domains: [web-frontend, ssg]
tags: [react-router, velite, static-site-generation]
curated: 2026-06-15
curated_by: config-scout
---

# Sansui233/blog-paper — claude-md

**Why it's worth keeping:** It explicitly explains the complex data flow between build-time (Velite processing) and runtime (SSG/CSR hybrid), which is critical for avoiding mistakes in static site generation.

**Summary:** A highly detailed technical blueprint for an SSG blog using React Router 7 and Velite.

**Source credibility:** A niche personal project with a respectable star count for its category.

**Recency:** Extremely current, utilizing bleeding-edge tech like React 19 and Tailwind v4.

**Source:** [Sansui233/blog-paper/CLAUDE.md](https://github.com/Sansui233/blog-paper/blob/b76b9b6dc2fdb572db43d8131c96cad859fe6754/CLAUDE.md) · 17★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AGENTs.md

This file provides guidance to coding agents when working with code in this repository.

## Project Overview

A minimalist black-and-white personal blog with micro-blogging (memos) functionality, built with React Router 7 in SSG mode.

## Commands

```bash
pnpm dev          # Start development server
pnpm build        # Build for production (SSG)
pnpm start        # Run production server
pnpm typecheck    # Generate types and run TypeScript check
```

## Architecture

### Tech Stack
- **React Router 7.11** with SSG (ssr: false, prerender enabled)
- **React 19** + **TypeScript 5.9**
- **Tailwind CSS v4** with Vite plugin
- **Velite** for Markdown/MDX content processing
- **Vite 7** as build tool
- **Zustand** for state management (theme, language)
- **i18next** for internationalization

### Key Directories
```
app/
├── routes/           # Route handlers (home, posts, memos, categories, tags, about)
├── components/       # React components organized by feature
│   ├── common/       # Shared (layout, topbar, footer, search, waline)
│   ├── home/         # Home page (ArticleItem, NavCat)
│   ├── post/         # Post page (FloatButtons, Pagination, PostMeta, TOC)
│   ├── me
```

</details>
