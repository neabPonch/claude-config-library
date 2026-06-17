---
name: mikecebul__bases
source: https://github.com/mikecebul/bases/blob/ab01dfddb7686f0044796182d72bb0f4af40a217/CLAUDE.md
repo: mikecebul/bases
kind: claude-md
stars: 42
last_pushed: 2026-03-17T05:01:59Z
license: mit
score: 8
domains: [web-frontend, fullstack, cms]
tags: [nextjs, payload-cms, block-based]
curated: 2026-06-16
curated_by: config-scout
---

# mikecebul/bases — claude-md

**Why it's worth keeping:** The 'Block System' and 'Collections' sections are excellent; they teach an agent what building blocks exist so it can extend the site using established patterns instead of inventing new ones. It also includes vital environment variable requirements for local setup.

**Summary:** Provides deep architectural context for a Next.js/PayloadCMS application, focusing on its block-based content system and role-based access control.

**Source credibility:** A practical, real-world small business template with recent maintenance history.

**Recency:** 

**Source:** [mikecebul/bases/CLAUDE.md](https://github.com/mikecebul/bases/blob/ab01dfddb7686f0044796182d72bb0f4af40a217/CLAUDE.md) · 42★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Next.js 15 application built with PayloadCMS for content management, serving as a business website template for substance and mental health counseling services. The project uses MongoDB for data storage and is designed to be a reusable boilerplate for small business websites.

## Development Commands

- **Development**: `pnpm run dev` - Start development server with turbo mode
- **Build**: `pnpm run build` - Run migrations and build for production
- **Type Check**: `pnpm run typecheck` - Run TypeScript type checking
- **Lint**: `pnpm run lint` - Run ESLint
- **Lint Fix**: `pnpm run lint:fix` - Run ESLint with auto-fix
- **Start Production**: `pnpm start` - Start production server
- **Generate Types**: `pnpm run generate:types` - Generate Payload types
- **Create Migration**: `pnpm run migrate:create` - Create new database migration

## Architecture

### Core Technologies
- **Framework**: Next.js 15 with React 19
- **CMS**: PayloadCMS 3.48.0 with MongoDB database
- **Styling**: TailwindCSS with Shadcn/ui components
- **Animations**: Fram
```

</details>
