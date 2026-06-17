---
name: Shpigford__studio
source: https://github.com/Shpigford/studio/blob/24d22c4ed0394b44b3ccc7612cc9bb70c8faf635/CLAUDE.md
repo: Shpigford/studio
kind: claude-md
stars: 139
last_pushed: 2026-03-27T21:22:21Z
license: mit
score: 9
domains: [web-frontend, creative-coding]
tags: [react, p5js, canvas, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# Shpigford/studio — claude-md

**Why it's worth keeping:** It prevents common AI errors by defining name disambiguation (p.random vs Math.random) and provides exact performance optimization strategies for canvas rendering loops.

**Summary:** A high-density technical guide for a generative art suite that enforces specific architectural patterns and p5.js instance mode constraints.

**Source credibility:** High-quality niche project with specific, expert-level technical nuances regarding p5.js v2 and React 19.

**Recency:** Extremely current; uses latest versions of React (19) and Tailwind (v4).

**Source:** [Shpigford/studio/CLAUDE.md](https://github.com/Shpigford/studio/blob/24d22c4ed0394b44b3ccc7612cc9bb70c8faf635/CLAUDE.md) · 139★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Unified Design Studio — a single web app consolidating 8 standalone generative art/design tools into one cohesive experience. Tools share UI components, theming, and utilities but each has its own canvas renderer and settings.

Detailed specs live in `docs/PLAN.md`. Treat it as the source of truth for architecture decisions, tool specs, and implementation phases.

## Stack

- **Vite + React 19 + TypeScript** (strict mode)
- **Tailwind CSS v4 + shadcn/ui** for UI controls
- **react-router-dom v7** for path-based routing (`/blocks`, `/topo`, etc.)
- **p5.js** (instance mode) for 7 tools, **Canvas 2D** for dither
- **mp4-muxer** for video export, **react-colorful** for color pickers
- **vitest** for utility tests

## Commands

```bash
npm run dev        # Vite dev server
npm run build      # Production build
npm run preview    # Preview production build
npm run lint       # Lint
npx tsc -b         # Type check (uses project references; `tsc --noEmit` checks nothing)
npx vitest run     # Run all tests
npx vitest run src/lib/color.test.ts  # Single te
```

</details>
