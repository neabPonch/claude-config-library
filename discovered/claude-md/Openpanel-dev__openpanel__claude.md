---
name: Openpanel-dev__openpanel__claude
source: https://github.com/Openpanel-dev/openpanel/blob/241d2597324cecd85a8354d3aa5482a7c9a5fb59/.claude/CLAUDE.md
repo: Openpanel-dev/openpanel
kind: claude-md
stars: 5931
last_pushed: 2026-06-13T10:43:29Z
license: agpl-3.0
score: 9
domains: [web-frontend, backend-api, fullstack]
tags: [monorepo, architecture-map, style-guide]
curated: 2026-06-15
curated_by: config-scout
---

# Openpanel-dev/openpanel — claude-md

**Why it's worth keeping:** The 'Data Flow' and 'Three-Database Strategy' sections provide critical architectural context to prevent the LLM from making wrong tool choices. It also includes a complete command list essential for autonomous agent workflows.

**Summary:** A comprehensive technical map that combines a project manual with strict coding standards for a complex monorepo.

**Source credibility:** High; highly starred, active open-source project with recent activity.

**Recency:** Extremely current, referencing React 19 and Tailwind v4.

**Source:** [Openpanel-dev/openpanel/.claude/CLAUDE.md](https://github.com/Openpanel-dev/openpanel/blob/241d2597324cecd85a8354d3aa5482a7c9a5fb59/.claude/CLAUDE.md) · 5931★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

NEVER CALL FORMAT! WE'LL FORMAT IN THE FUTURE WHEN WE HAVE MERGED ALL BIG PRS!

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Openpanel is an open-source web/product analytics platform (Mixpanel alternative). It's a **pnpm monorepo** with apps, packages, tooling, and SDKs.

## Common Commands

```bash
# Development
pnpm dev                    # Run all services (api, worker, dashboard) in parallel
pnpm dev:public             # Run public/docs site only
pnpm dock:up / dock:down    # Start/stop Docker (PostgreSQL, Redis, ClickHouse)

# Code quality
pnpm check                  # Lint check (Biome via Ultracite)
pnpm fix                    # Auto-fix lint/format issues
pnpm typecheck              # Typecheck all packages

# Testing
pnpm test                   # Run all tests (vitest)
pnpm vitest run <path>      # Run a single test file
# Workspace: packages/* and apps/* (excluding apps/start)

# Database
pnpm codegen                # Generate Prisma types + geo data
pnpm migrate                # Run Prisma migrations (dev)
pnpm migrate:deploy         # Deploy migrations (production - never run t
```

</details>
