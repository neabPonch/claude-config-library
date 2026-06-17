---
name: 4NTP__hanul
source: https://github.com/4NTP/hanul/blob/16457947b2315055a6241e75b6fac4f8cd70c172/CLAUDE.md
repo: 4NTP/hanul
kind: claude-md
stars: 0
last_pushed: 2025-08-24T01:48:31Z
license: unknown
score: 9
domains: [fullstack, monorepo, web-frontend, backend-api]
tags: [turborepo, nestjs, nextjs, prisma, zod]
curated: 2026-06-17
curated_by: config-scout
---

# 4NTP/hanul — claude-md

**Why it's worth keeping:** Excellent use of 'never' constraints (e.g., banning raw fetch) and specific workflow sequences for schema changes, which prevents AI from making common architectural errors.

**Summary:** A highly detailed guide for a full-stack Turborepo comprising NestJS and Next.js applications.

**Source credibility:** Low social proof due to 0 stars, but the technical depth suggests an experienced professional author.

**Recency:** Very current, referencing Next.js 15 and modern full-stack patterns.

**Source:** [4NTP/hanul/CLAUDE.md](https://github.com/4NTP/hanul/blob/16457947b2315055a6241e75b6fac4f8cd70c172/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a full-stack monorepo called "Hanul" using Turborepo with two main applications:

- **Server** (`apps/server`): NestJS API with PostgreSQL database via Prisma ORM
- **Web** (`apps/web`): Next.js frontend with internationalization and Tailwind CSS

## Common Development Commands

Use these commands from the root directory:

```bash
# Install dependencies
pnpm install

# Start development servers (both apps)
pnpm dev

# Build all applications
pnpm build

# Run tests across all packages
pnpm test

# Lint all code
pnpm lint

# Format all code
pnpm format

# Type check all packages
pnpm check-types
```

### Server-specific commands (from apps/server):

```bash
# Start server in development
pnpm dev

# Start server in debug mode
pnpm start:debug

# Run unit tests
pnpm test

# Run E2E tests
pnpm test:e2e

# Generate Prisma client after schema changes
npx prisma generate

# Run database migrations
npx prisma migrate dev

# Reset database
npx prisma migrate reset
```

### Web-specific commands (from apps/web):

```bash
# Start web app in developme
```

</details>
