---
name: Fasttify__fasttify__claude
source: https://github.com/Fasttify/fasttify/blob/981470857208f8efd4545d89d4f274467ce55a33/.claude/CLAUDE.md
repo: Fasttify/fasttify
kind: claude-md
stars: 12
last_pushed: 2026-03-17T20:40:06Z
license: other
score: 9
domains: [web-frontend, backend-api, cloud-infrastructure]
tags: [nextjs, aws-amplify, multitenancy, monorepo]
curated: 2026-06-15
curated_by: config-scout
---

# Fasttify/fasttify — claude-md

**Why it's worth keeping:** It provides specific architectural guardrails (like the storeId partitioning rule) and boilerplate code patterns that prevent common logic errors in a multi-tenant environment.

**Summary:** A highly detailed technical manual covering build commands, monorepo architecture, and critical multi-tenant data patterns.

**Source credibility:** The repository is active and uses a sophisticated modern stack, indicating high-quality manual documentation.

**Recency:** Extremely current, referencing Next.js 16 and AWS Amplify Gen2.

**Source:** [Fasttify/fasttify/.claude/CLAUDE.md](https://github.com/Fasttify/fasttify/blob/981470857208f8efd4545d89d4f274467ce55a33/.claude/CLAUDE.md) · 12★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Fasttify is a multi-tenant SaaS platform for creating and managing online stores with a Liquid template engine 100% compatible with Shopify. The project is built with Next.js 16, AWS Amplify Gen2, and uses a monorepo structure with pnpm workspaces.

## Build & Development Commands

### Core Commands

```bash
# Install dependencies (required first step)
pnpm install

# Start AWS Amplify sandbox (local backend)
npx ampx sandbox --identifier <YOUR_NAME> --stream-function-logs

# Development server with Turbopack
pnpm run dev

# Production build (optimized with Turbopack)
pnpm run build:fast

# Full production build (includes type-checking)
pnpm run build:full

# Start production server
pnpm run start
```

### Testing & Quality

```bash
# Run all tests
pnpm run test

# Run tests in watch mode
pnpm run test:watch

# Generate coverage report
pnpm run test:coverage

# Type-check entire codebase
pnpm run type-check

# Fast type-check (skip lib checks)
pnpm run type-check:fast

# Lint all files
pnpm run lint

# Auto-fix lint errors
pnpm run lint:fix

# Li
```

</details>
