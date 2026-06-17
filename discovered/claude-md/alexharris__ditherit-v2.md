---
name: alexharris__ditherit-v2
source: https://github.com/alexharris/ditherit-v2/blob/852f278e49b3675b38c4c4d31ae89c52b200b47d/CLAUDE.md
repo: alexharris/ditherit-v2
kind: claude-md
stars: 260
last_pushed: 2026-04-21T05:13:12Z
license: unknown
score: 8
domains: [web-frontend, image-processing]
tags: [vue, nuxt, architecture-map]
curated: 2026-06-15
curated_by: config-scout
---

# alexharris/ditherit-v2 — claude-md

**Why it's worth keeping:** Maps core business flows to specific files and includes critical warnings about a custom dependency fork and Node.js version requirements.

**Summary:** Provides a clear functional decomposition of the app's logic and essential environment setup instructions.

**Source credibility:** Personal project with high technical specificity and recent maintenance.

**Recency:** 

**Source:** [alexharris/ditherit-v2/CLAUDE.md](https://github.com/alexharris/ditherit-v2/blob/852f278e49b3675b38c4c4d31ae89c52b200b47d/CLAUDE.md) · 260★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Dither it! is a client-side image dithering web app built with **Vue 2 / Nuxt 2** (SPA mode, `ssr: false`). It uses [RgbQuant.js](https://github.com/leeoniya/RgbQuant.js) (custom fork with transparency support) for color quantization and dithering, with Canvas API for image rendering.

## Commands

```bash
# Dev server (localhost:3000) — requires Node <17 or setting legacy OpenSSL first
export NODE_OPTIONS=--openssl-legacy-provider  # needed for Node.js v17+
npm run dev

# Build & start production server
npm run build && npm run start

# Generate static site to /docs (GitHub Pages)
npm run generate
npm run generate:gh-pages  # with DEPLOY_ENV=GH_PAGES

# Lint
npm run lint

# Test
npm run test
```

## Architecture

**SPA with file-based routing** — Nuxt 2 with SSR disabled. Static output goes to `/docs`.

### Core Processing Flow

1. `components/ImageUpload.vue` — handles file input, drag-drop, clipboard paste
2. `pages/index.vue` (~1000 lines) — **the main application logic**: dithering configuration, RgbQuant invocation, Canvas rendering, downlo
```

</details>
