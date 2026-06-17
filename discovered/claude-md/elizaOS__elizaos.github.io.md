---
name: elizaOS__elizaos.github.io
source: https://github.com/elizaOS/elizaos.github.io/blob/838529c24739284153d6c399467a9dc9cc067e9b/CLAUDE.md
repo: elizaOS/elizaos.github.io
kind: claude-md
stars: 106
last_pushed: 2026-06-14T23:47:27Z
license: mit
score: 9
domains: [data-pipeline, web-frontend, cli-tools]
tags: [nextjs, typescript, bun, data-processing]
curated: 2026-06-15
curated_by: config-scout
---

# elizaOS/elizaos.github.io — claude-md

**Why it's worth keeping:** The detailed 'Pipeline Commands' section and the 'Key Architecture' explanation provide crucial context for how data flows through the system. It also includes specific environment variable requirements that are critical for running non-standard tasks.

**Summary:** This file provides an exceptional breakdown of a dual-purpose project containing both a Next.js frontend and a complex data processing pipeline. It clearly explains how the two systems interact through specialized CLI commands.

**Source credibility:** Highly credible; part of a high-activity, well-maintained ecosystem (elizaOS).

**Recency:** Very current; uses modern technologies like Next.js 15 and Bun.

**Source:** [elizaOS/elizaos.github.io/CLAUDE.md](https://github.com/elizaOS/elizaos.github.io/blob/838529c24739284153d6c399467a9dc9cc067e9b/CLAUDE.md) · 106★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

GitHub Contributor Analytics platform for tracking, analyzing, and visualizing repository contributions. Features include:

- Daily, weekly, and monthly reports on repository activity
- Contributor profile pages with metrics and visualizations
- Activity tracking for PRs, issues, and commits
- Configurable scoring system for ranking contributors
- AI-powered activity summaries

## Tech Stack

- Frontend: Next.js 15, React, TypeScript, Tailwind CSS, shadcn/ui
- Data Processing: TypeScript pipeline with SQLite/Drizzle ORM
- Automation: GitHub Actions for scheduled reports

## Build & Development Commands

```bash
bun run dev          # Start development server
bun run build        # Build production site
bun run check        # Run linter and type checks
bun run lint         # Run ESLint only
bun run db:generate  # Generate database schema
bun run db:migrate   # Run database migrations
bun run db:studio    # Launch Drizzle studio
```

## Pipeline Commands

```bash
# Data Ingestion
bun run pipeline ingest              # Ingest latest GitHub data (def
```

</details>
