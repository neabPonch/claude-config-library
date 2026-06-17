---
name: jishono__jishono-front
source: https://github.com/jishono/jishono-front/blob/e1378ac0fd8114ec8ea025540b22cd634526394b/CLAUDE.md
repo: jishono/jishono-front
kind: claude-md
stars: 7
last_pushed: 2026-06-14T03:59:06Z
license: unknown
score: 8
domains: [web-frontend, vuejs]
tags: [architecture, data-mapping, environment-config]
curated: 2026-06-15
curated_by: config-scout
---

# jishono/jishono-front — claude-md

**Why it's worth keeping:** It maps specific data model fields to template usage and documents crucial global dependencies (jQuery/Bootstrap) that would otherwise confuse an AI agent.

**Summary:** Detailed architecture overview for a Vue 3 SPA, covering environmental setup and specific client-side search patterns.

**Source credibility:** Small specialized repository; documentation is clearly hand-written and highly specific to the business logic.

**Recency:** Current; uses modern Vite and Vue 3 standards.

**Source:** [jishono/jishono-front/CLAUDE.md](https://github.com/jishono/jishono-front/blob/e1378ac0fd8114ec8ea025540b22cd634526394b/CLAUDE.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
npm run dev      # Start dev server (Vite, default port 5173)
npm run build    # Production build to dist/
npm run preview  # Preview production build
```

No test suite is configured.

## Environment

- `.env` — dev: `VITE_NODE_HOST=http://localhost:3001/`
- `.env.production` — prod: `VITE_NODE_HOST=https://api.jisho.no`

The backend API must be running locally on port 3001 for development.

## Architecture

This is a Vue 3 SPA for [jisho.no](https://www.jisho.no), a Norwegian–Japanese online dictionary. Built with Vite, Vue Router, vue-i18n, and Axios.

**Key design: client-side search.** On startup, `Search.vue` fetches the entire word list from `GET /items/all` and stores it in memory. All filtering and sorting happens client-side by matching `item.oppslag` against the query string. Example sentences (`GET /example_sentences/:id`) and conjugations (`POST /conjugations/:id`) are fetched lazily on demand.

**Data model fields used in templates:**
- `oppslag` — Norwegian headword
- `lemma_id` — unique word ID
- `definisjoner` — array of definiti
```

</details>
