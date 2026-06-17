---
name: open4good__open4goods__claude
source: https://github.com/open4good/open4goods/blob/a4dbdcca856b065cdf53a54f79a36da2f752a888/frontend/CLAUDE.md
repo: open4good/open4goods
kind: claude-md
stars: 29
last_pushed: 2026-06-15T05:48:45Z
license: other
score: 9
domains: [web-frontend, nuxt-js]
tags: [nuxt, vue, typescript, api-generation]
curated: 2026-06-15
curated_by: config-scout
---

# open4good/open4goods — claude-md

**Why it's worth keeping:** Includes 'Key Patterns' that explain business logic (auth/roles) rather than just syntax, and provides explicit instructions for critical workflows like regenerating the OpenAPI client.

**Summary:** Provides detailed context for a Nuxt 3 application, including specific commands, directory structures, and architectural patterns.

**Source credibility:** Active repository with recent commits and a moderate star count indicating real-world usage.

**Recency:** Very current; uses modern tools like pnpm 10 and includes specific MCP server instructions.

**Source:** [open4good/open4goods/frontend/CLAUDE.md](https://github.com/open4good/open4goods/blob/a4dbdcca856b065cdf53a54f79a36da2f752a888/frontend/CLAUDE.md) · 29★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Package Manager

This project uses `pnpm` as the package manager. All commands should be run with `pnpm`.

### Essential Commands

- `pnpm dev` - Start development server (http://localhost:3000)
- `pnpm build` - Production build
- `pnpm build:ssr` - Production build with increased memory (NODE_OPTIONS='--max-old-space-size=8192')
- `pnpm generate` - Static site generation
- `pnpm preview` - Serve production build locally
- `pnpm lint` - Run ESLint
- `pnpm lint:fix` - Run ESLint and fix issues + Prettier formatting
- `pnpm format` - Run Prettier formatting
- `pnpm format:check` - Check Prettier formatting
- `pnpm test` - Run Vitest tests
- `pnpm generate:api` - Regenerate OpenAPI client from remote spec
- `pnpm preprocess:css` - Process Bootstrap/XWiki styles for TextContent component

### Prerequisites

- Node.js >=20
- pnpm 10.12.1 (install with `npm install -g pnpm@10.12.1`)

## Architecture Overview

This is a **Nuxt 3** frontend application built with **Vue 3** and **TypeScript**. Key architectural patterns:

### Core Stack

- **Nuxt
```

</details>
