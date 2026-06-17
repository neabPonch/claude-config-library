---
name: mmarinovic__React2AWS
source: https://github.com/mmarinovic/React2AWS/blob/4497e9b0dbeedaec749fa0f2adebefc5bf5b0898/CLAUDE.md
repo: mmarinovic/React2AWS
kind: claude-md
stars: 442
last_pushed: 2026-01-24T18:26:07Z
license: unknown
score: 8
domains: [web-frontend, infrastructure-as-code]
tags: [bun, nextjs, terraform, architecture-map]
curated: 2026-06-14
curated_by: config-scout
---

# mmarinovic/React2AWS — claude-md

**Why it's worth keeping:** The component-to-generator mapping table is a top-tier technique for helping agents navigate complex logic without scanning every file; the 'No TODO/FIXME' rule also prevents low-quality AI completions.

**Summary:** A highly structured guide that maps high-level business components directly to their implementation files and enforces strict architectural boundaries.

**Source credibility:** Strong; 442 stars and recent updates indicate a high-quality, real-world project.

**Recency:** Highly current; uses modern Bun and Next.js App Router patterns relevant to today's workflows.

**Source:** [mmarinovic/React2AWS/CLAUDE.md](https://github.com/mmarinovic/React2AWS/blob/4497e9b0dbeedaec749fa0f2adebefc5bf5b0898/CLAUDE.md) · 442★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to AI coding agents working in this repository.

## Project Overview

**React2AWS** transforms React JSX syntax into production-ready Terraform code for AWS infrastructure. Users write familiar JSX with Tailwind-style className configuration and get complete Terraform projects. The main components are the landing page (marketing), the studio (live editor with preview), and the generator engine (JSX parsing and Terraform generation).

## Development Commands

**Package Management:**

- Use `bun` - never use npm or yarn
- `bun install` - Install dependencies

**Development:**

- `bun run dev` - Run the Next.js dev server (localhost:3000)
- `bun run build` - Build for production
- `bun run start` - Start production server

**Testing:**

- `bun test` - Run unit tests
- `bun test --watch` - Run tests in watch mode
- `bun test --coverage` - Run tests with coverage
- `bun run test:e2e` - Run Playwright E2E tests
- `bun run test:e2e:ui` - Run E2E tests with Playwright UI
- `bun run test:e2e:headed` - Run E2E tests in headed browser

**Code Quality:**

- `bun run lint` - Run ESLint

## Architecture Overview

**Pages:**

- `src/app/page.tsx` - Landing
```

</details>
