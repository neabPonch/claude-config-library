---
name: skillrecordings__egghead-next
source: https://github.com/skillrecordings/egghead-next/blob/974834210efbb9bdb1f1cfcf01e40fe0996f4a09/CLAUDE.md
repo: skillrecordings/egghead-next
kind: claude-md
stars: 1448
last_pushed: 2026-06-14T23:23:20Z
license: other
score: 9
domains: [web-frontend, nextjs]
tags: [architecture, patterns, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# skillrecordings/egghead-next — claude-md

**Why it's worth keeping:** The 'Preferred Code Organization Structure' gives explicit rules for file decomposition that guide an AI toward maintainable patterns. The detailed MySQL connection pattern is a high-value guardrail against breaking server-only logic.

**Summary:** Provides comprehensive architectural guidelines, command lists, and specific code organization patterns for a large Next.js application. It includes critical technical warnings regarding database connectivity to prevent client-side import errors.

**Source credibility:** High; sourced from a highly-starred, actively maintained professional repository.

**Recency:** Very current, utilizing modern Next.js 14 and TypeScript standards.

**Source:** [skillrecordings/egghead-next/CLAUDE.md](https://github.com/skillrecordings/egghead-next/blob/974834210efbb9bdb1f1cfcf01e40fe0996f4a09/CLAUDE.md) · 1448★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the Next.js frontend for egghead.io, an online learning platform. It requires the `egghead-rails` backend to be running for full functionality.

## Essential Commands

```bash
# Install dependencies (MUST use pnpm)
pnpm install

# Development
pnpm dev              # Start Next.js dev server on port 3000
pnpm dev:concurrent   # Run dev server + Inngest dev server

# Testing
pnpm test            # Run tests in watch mode
pnpm test:ci         # Run tests once (for CI)

# Code Quality
pnpm lint            # Run ESLint with auto-fix
pnpm format          # Run Prettier on all files
pnpm build           # Production build (also runs type checking)

# Sanity CMS
pnpm sanity          # Start Sanity Studio
```

## Architecture Overview

### Tech Stack

- **Framework**: Next.js 14.2.4 with React 18.3.1
- **Language**: TypeScript with strict mode
- **Styling**: Tailwind CSS + CSS Modules
- **State Management**: XState (state machines), React hooks, tRPC (server state)
- **Database**: Postgres
- **CMS**: Sanity
- **Video**: Mux
- **Payments**: Stripe
```

</details>
