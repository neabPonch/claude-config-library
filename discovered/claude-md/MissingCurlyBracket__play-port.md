---
name: MissingCurlyBracket__play-port
source: https://github.com/MissingCurlyBracket/play-port/blob/323746c819c82e946afedb7a29afc87a07a083e5/CLAUDE.md
repo: MissingCurlyBracket/play-port
kind: claude-md
stars: 0
last_pushed: 2026-05-02T13:59:50Z
license: unknown
score: 8
domains: [web-frontend, serverless, fullstack]
tags: [react, aws-lambda, atomic-design, tanstack]
curated: 2026-06-15
curated_by: config-scout
---

# MissingCurlyBracket/play-port — claude-md

**Why it's worth keeping:** It provides critical context on design patterns (Atomic Design) and includes explicit warnings about auto-generated files to prevent the AI from attempting manual edits that break build processes.

**Summary:** A comprehensive guide for a fullstack React and AWS Lambda application including detailed architectural patterns.

**Source credibility:** Low star count, but shows high-quality technical documentation for a specific project.

**Recency:** Very current, referencing modern technologies like React 19 and TanStack Router.

**Source:** [MissingCurlyBracket/play-port/CLAUDE.md](https://github.com/MissingCurlyBracket/play-port/blob/323746c819c82e946afedb7a29afc87a07a083e5/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Play-port is a streaming service locator that helps users find where to watch movies and TV shows. It has a React SPA frontend deployed to GitHub Pages and an AWS Lambda serverless backend that proxies the TMDB (The Movie Database) API.

## Commands

| Task | Command |
|---|---|
| Dev server | `npm run dev` |
| Build | `npm run build` (runs `tsc -b && vite build`) |
| Lint | `npm run lint` |
| Type check | `npm run typecheck` |
| Run tests | `npm run test` |
| Run tests with UI | `npm run test:ui` |
| Run single test | `npx vitest run path/to/file.test.ts` |
| Local backend | `npx serverless offline` |
| Deploy | `npm run deploy` (GitHub Pages) |

## Architecture

### Frontend (`/src`)

- **React 19 + TypeScript + Vite** with TanStack Router (file-based routing) and TanStack React Query for server state
- **Styling**: Tailwind CSS + Material-UI (MUI)
- **Atomic design** component structure: `components/atoms/` (MUI wrappers like BaseButton, BaseBox), `components/molecules/` (SearchBar, TitleItem, RegionSelect), `components/organisms/` (Preference
```

</details>
