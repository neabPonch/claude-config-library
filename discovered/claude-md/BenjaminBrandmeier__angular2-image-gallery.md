---
name: BenjaminBrandmeier__angular2-image-gallery
source: https://github.com/BenjaminBrandmeier/angular2-image-gallery/blob/dbc98b9163dae9887d871c0ba613aacc047d7864/CLAUDE.md
repo: BenjaminBrandmeier/angular2-image-gallery
kind: claude-md
stars: 305
last_pushed: 2026-02-08T05:50:20Z
license: mit
score: 8
domains: [web-frontend, angular, monorepo]
tags: [angular, monorepo, build-steps, image-processing]
curated: 2026-06-16
curated_by: config-scout
---

# BenjaminBrandmeier/angular2-image-gallery — claude-md

**Why it's worth keeping:** Explains a critical build-order dependency (building the lib before running the demo) and details a non-obvious image processing pipeline using external scripts.

**Summary:** Provides essential context for a monorepo involving an Angular library and its consuming demo application.

**Source credibility:** Reliable niche project with decent star count and recent activity.

**Recency:** Current; uses modern Angular terminology and targets Claude Code effectively.

**Source:** [BenjaminBrandmeier/angular2-image-gallery/CLAUDE.md](https://github.com/BenjaminBrandmeier/angular2-image-gallery/blob/dbc98b9163dae9887d871c0ba613aacc047d7864/CLAUDE.md) · 305★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Monorepo containing an Angular 21 responsive image gallery library (`angular2-image-gallery`) and its demo application. The library is published to npm and handles high-resolution image display with multi-resolution support.

## Commands

- **Dev server**: `npm start` (or `npm run start-net` for network access)
- **Build library**: `npm run lib` (builds via ng-packagr, copies convert script and README to dist)
- **Build demo app**: `npm run build`
- **Run tests**: `npm test`
- **Lint**: `npm run lint`
- **E2E tests**: `npm run e2e`

The demo app depends on the built library (`"angular2-image-gallery": "file:dist/angular2-image-gallery"`), so you must run `npm run lib` before `npm start` if the library hasn't been built yet.

## Architecture

### Two-project structure

- **`projects/angular2-image-gallery/`** - The reusable library (built with ng-packagr)
  - `gallery/` - Grid layout component with responsive row-based image arrangement
  - `viewer/` - Full-screen image viewer with keyboard/touch navigation and quality selection
  - `services/imag
```

</details>
