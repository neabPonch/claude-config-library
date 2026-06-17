---
name: MrModest__reisenotiz__claude
source: https://github.com/MrModest/reisenotiz/blob/9596dd9411e654aae2b4eb57bde5b3cd82a269a1/apps/frontend/CLAUDE.md
repo: MrModest/reisenotiz
kind: claude-md
stars: 62
last_pushed: 2026-06-14T16:10:28Z
license: other
score: 8
domains: [web-frontend, react]
tags: [react-19, tailwind-v4, typescript, vite]
curated: 2026-06-15
curated_by: config-scout
---

# MrModest/reisenotiz — claude-md

**Why it's worth keeping:** The 'Custom Instructions' section provides critical, highly specific guidance to prevent the LLM from using deprecated React 19 patterns like forwardRef. It also enforces a strict pattern for icon usage and design system compliance.

**Summary:** This config defines a strict technical environment for a modern React 19 and Tailwind v4 frontend. It covers project structure, path aliases, and specific component patterns.

**Source credibility:** Solid; based on an active repository with decent star count suggesting real-world application use.

**Recency:** 

**Source:** [MrModest/reisenotiz/apps/frontend/CLAUDE.md](https://github.com/MrModest/reisenotiz/blob/9596dd9411e654aae2b4eb57bde5b3cd82a269a1/apps/frontend/CLAUDE.md) · 62★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Frontend

This file applies when working inside `apps/frontend/`. Run all commands from this directory.

## Working Directory

All paths in this document are relative to `apps/frontend/`. The `@/` alias points to `apps/frontend/src/`.

---

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

- `pnpm dev` - Start Vite development server
- `pnpm build` - Type-check with TypeScript and build for production
- `pnpm lint` - Run ESLint on TypeScript/TSX files
- `pnpm preview` - Preview production build locally

## Architecture Overview

### Tech Stack
- **Framework**: React 19 with Vite build tool
- **Routing**: React Router v7 with nested routes
- **Styling**: Tailwind CSS v4 (using @tailwindcss/vite plugin)
- **Date/Time**: Luxon wrapped in custom DateTime class (`src/lib/datetime/`)
- **Animations**: Motion (Framer Motion) library
- **Component Patterns**:
  - Reusing existing shadcn components whenever feasible
  - Class-variance-authority (CVA) for component variants
  - Base UI primitives
  - Lucide React for icons
- **PWA**: Progressive Web App with vite-plugin-pwa and Workbox
- **React Comp
```

</details>
