---
name: adamkali__mindscape__claude
source: https://github.com/adamkali/mindscape/blob/f799fc1af7fc76da3d6e84ac2639ed0039e5a413/web/CLAUDE.md
repo: adamkali/mindscape
kind: claude-md
stars: 0
last_pushed: 2026-06-06T13:21:27Z
license: unknown
score: 8
domains: [web-frontend, api-integration]
tags: [solidjs, typescript, tailwind-4, openapi, rsbuild]
curated: 2026-06-15
curated_by: config-scout
---

# adamkali/mindscape — claude-md

**Why it's worth keeping:** The detailed breakdown of the generated API structure (models vs. classes) and path aliases allows an agent to perform complex data-fetching tasks without manual discovery.

**Summary:** Provides a high-density technical overview of a SolidJS frontend, specifically focusing on the auto-generated API client and build tool configuration.

**Source credibility:** Low/Unknown; repository has 0 stars and no established reputation.

**Recency:** Extremely current, utilizing modern tools like TailwindCSS 4.x and Rsbuild.

**Source:** [adamkali/mindscape/web/CLAUDE.md](https://github.com/adamkali/mindscape/blob/f799fc1af7fc76da3d6e84ac2639ed0039e5a413/web/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

- **Start development server**: `pnpm dev` (runs on http://localhost:5173)
- **Build for production**: `pnpm build`
- **Preview production build**: `pnpm preview`
- **Format code**: `pnpm format` (uses Biome)
- **Lint and format**: `pnpm check` (uses Biome with auto-fix)

## Architecture Overview

This is a SolidJS frontend application built with Rsbuild that communicates with a Go backend API called "mindscape". The project structure follows a clear separation of concerns:

### Tech Stack
- **Frontend Framework**: SolidJS with TypeScript
- **Build Tool**: Rsbuild with Solid plugin
- **Styling**: TailwindCSS 4.x
- **Code Quality**: Biome (formatter + linter)
- **Package Manager**: pnpm

### API Integration
- Auto-generated TypeScript API client from OpenAPI/Swagger spec
- Located in `src/api/` with models and API classes
- Backend proxy configured to `http://0.0.0.0:60000` for `/api` and `/assets` routes
- Uses JWT authorization headers for authenticated endpoints

### Key API Features
- User authentication (login/signup)
- User management (C
```

</details>
