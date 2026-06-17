---
name: will-be-done__will-be-done__no-claude
source: https://github.com/will-be-done/will-be-done/blob/84224e16e2fcd237228cb807ba9178217cd492d4/no-CLAUDE.md
repo: will-be-done/will-be-done
kind: claude-md
stars: 89
last_pushed: 2026-06-14T10:56:46Z
license: agpl-3.0
score: 9
domains: [web-frontend, backend-api, monorepo]
tags: [architecture, monorepo, typescript, fullstack]
curated: 2026-06-15
curated_by: config-scout
---

# will-be-done/will-be-done — claude-md

**Why it's worth keeping:** The explicit explanation of project-specific patterns (like dot-notation routing or fractional indexing) prevents AI hallucination/error. The detailed directory structures serve as a high-density map for navigating the monorepo.

**Summary:** This config provides deep architectural context for a complex monorepo, covering development commands, tech stacks, and core business logic. It effectively maps out component hierarchies and explains specialized systems like the synchronization engine.

**Source credibility:** High; an active, recently updated repository with significant star count and clear ownership.

**Recency:** Highly current, referencing modern stacks like React 19 and Vite 7.

**Source:** [will-be-done/will-be-done/no-CLAUDE.md](https://github.com/will-be-done/will-be-done/blob/84224e16e2fcd237228cb807ba9178217cd492d4/no-CLAUDE.md) · 89★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Root Level Commands
- `bun dev:client` - Start the web client in development mode (Vite dev server)
- `bun dev:server` - Start the API server in development mode (Fastify + Bun)

### Web Client (apps/web/)
- `bun dev` - Start Vite development server with React 19
- `bun build` - Build for production (TypeScript check + Vite build)
- `bun ts` - Run TypeScript compiler check
- `bun lint` - Run ESLint
- `bun lint:fix` - Run ESLint with auto-fix
- `bun test` - Run Vitest tests
- `bun format` - Format code with Prettier

### API Server (apps/api/)
- `bun dev` - Start development server with Bun (runs src/start.ts)

### Slices Library (apps/slices/)
- `bun ts` - Run TypeScript compiler check

## Architecture Overview

This is a **monorepo task management application** with a shared state management system across client and server.

### Applications Structure

#### `apps/web` - React 19 Client
The frontend application built with modern React and TypeScript.

**Key Technologies:**
- **Framework**: React 19 with React Compiler (babel-plugin-react-
```

</details>
