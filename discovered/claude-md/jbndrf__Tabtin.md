---
name: jbndrf__Tabtin
source: https://github.com/jbndrf/Tabtin/blob/ee01f4cbda97b1e9acd7c037368572c5ce070817/CLAUDE.md
repo: jbndrf/Tabtin
kind: claude-md
stars: 4
last_pushed: 2026-02-20T00:01:27Z
license: unknown
score: 8
domains: [web-frontend, backend-api, fullstack]
tags: [sveltekit, pocketbase, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# jbndrf/Tabtin — claude-md

**Why it's worth keeping:** Specifies exact tech versions (Svelte 5 runes, Tailwind 4) to prevent syntax errors and maps out the data flow/directory structure for efficient navigation.

**Summary:** Provides a comprehensive architectural overview of a SvelteKit and PocketBase full-stack application.

**Source credibility:** Real-world project with recent maintenance activity.

**Recency:** Very current; utilizes modern frameworks like Svelte 5 and Tailwind 4.

**Source:** [jbndrf/Tabtin/CLAUDE.md](https://github.com/jbndrf/Tabtin/blob/ee01f4cbda97b1e9acd7c037368572c5ce070817/CLAUDE.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Tabtin** - A self-hostable, mobile-first web app for extracting structured data from images using vision LLMs. Users define table schemas (columns), upload images, and the app extracts data into spreadsheet-like tables with review workflows.

## Development Commands

```bash
# Start frontend dev server (localhost:5173)
npm run dev

# Start PocketBase backend (localhost:8090)
npm run backend

# Build frontend for production
npm run build

# Build Go backend
npm run build:backend

# Run type checking
npm run check

# Regenerate PocketBase TypeScript types after schema changes
npm run typegen

# Format code
npm run format

# Lint
npm run lint
```

Development requires running both `npm run backend` and `npm run dev` in separate terminals.

## Architecture

### Tech Stack
- **Frontend**: SvelteKit 5 with Svelte 5 (runes), TypeScript, TailwindCSS 4
- **Backend**: PocketBase (Go) with custom extensions
- **UI Components**: shadcn-svelte (bits-ui based)
- **Forms**: sveltekit-superforms + Zod validation
- **i18n**: Paraglide JS (en/de locales in `mess
```

</details>
