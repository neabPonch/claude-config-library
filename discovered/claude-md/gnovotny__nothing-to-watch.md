---
name: gnovotny__nothing-to-watch
source: https://github.com/gnovotny/nothing-to-watch/blob/d5acf46805f0a9852d1c6e10b556ddca1c6295e9/CLAUDE.md
repo: gnovotny/nothing-to-watch
kind: claude-md
stars: 455
last_pushed: 2025-08-20T08:52:33Z
license: other
score: 8
domains: [web-frontend, webgl, visualization]
tags: [react, bun, webgl, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# gnovotny/nothing-to-watch — claude-md

**Why it's worth keeping:** The inclusion of 'Data Flow' and high-level component responsibility mapping (e.g., the integration layer vs. engine) allows an AI to reason about system interactions rather than just file contents.

**Summary:** Provides comprehensive technical context for a custom WebGL/React stack, including specific command nuances and architectural boundaries.

**Source credibility:** 455 stars indicates a respected, high-quality experimental project.

**Recency:** Extremely current, utilizing React 19, Bun, and Biome.

**Source:** [gnovotny/nothing-to-watch/CLAUDE.md](https://github.com/gnovotny/nothing-to-watch/blob/d5acf46805f0a9852d1c6e10b556ddca1c6295e9/CLAUDE.md) · 455★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

- `bun dev` - Start development server on port 3000
- `bun build` - Build the application with TypeScript compilation
- `bun preview` - Preview the built application
- `bun lint` - Lint code with Biome
- `bun format` - Format code with Biome  
- `bun check` - Run Biome checks (lint + format)
- `bun check:write` - Auto-fix Biome issues with unsafe fixes
- `bun analyze` - Build with bundle analysis enabled

## Testing Commands

- `bun run test` - Run unit tests with Vitest (use `bun run test`, not `bun test`)
- `bun test:unit` - Run unit tests with Vitest  
- `bun test:unit:coverage` - Run unit tests with coverage report
- `bun test:e2e` - Run end-to-end tests with Playwright
- `bun test:e2e:headed` - Run E2E tests in headed mode (visible browser)
- `bun test:e2e:ui` - Run E2E tests with Playwright UI

## Architecture Overview

This is a React application that visualizes film data using WebGL and a custom Voronoi force simulation called "Voroforce". The app renders thousands of film posters in an interactive force-directed diagram.

### Key Com
```

</details>
