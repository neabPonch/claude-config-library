---
name: AhmedElywa__prisma-tools
source: https://github.com/AhmedElywa/prisma-tools/blob/462851c5a03412fc58e252c2139a8cb08017911f/CLAUDE.md
repo: AhmedElywa/prisma-tools
kind: claude-md
stars: 699
last_pushed: 2026-06-11T06:44:45Z
license: mit
score: 9
domains: [monorepo, backend-infrastructure, cli-tools]
tags: [bun, prisma, monorepo, typescript]
curated: 2026-06-14
curated_by: config-scout
---

# AhmedElywa/prisma-tools — claude-md

**Why it's worth keeping:** Explicitly documents technical gotchas (like the bun publish vs workspace protocol issue) which prevents an AI from making critical toolchain errors.

**Summary:** A highly detailed guide for a Bun-based monorepo that covers complex build orders and specific publishing workflows.

**Source credibility:** High; well-starred, actively maintained open-source toolkit.

**Recency:** Very recent; incorporates cutting-edge standards like Prisma 7 and React 19.

**Source:** [AhmedElywa/prisma-tools/CLAUDE.md](https://github.com/AhmedElywa/prisma-tools/blob/462851c5a03412fc58e252c2139a8cb08017911f/CLAUDE.md) · 699★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

PalJS is a comprehensive toolkit for building NodeJS, Prisma, GraphQL, and React applications. It's organized as a monorepo using bun workspaces, providing code generation, admin interfaces, and query optimization tools.

**Current version**: v9 (beta) — Prisma 7 compatible, native Prisma generator.

## Commands

### Development Commands

```bash
# Install dependencies (using bun)
bun install

# Add new packages
bun add [package-name]
bun add -D [dev-package-name]

# Add packages to specific workspace
bun add [package-name] --filter @paljs/[workspace-name]

# Build all v9 packages in dependency order
bun run build

# Run tests (excludes Playwright E2E specs)
bun run test

# Lint and format code with biome
bun run check        # Check for issues
bun run check:fix    # Auto-fix issues
bun run lint         # Lint only
bun run format       # Format code
bun run format:ci    # Check formatting (CI)

# Generate documentation
bun run docs:gen
```

### Package-Specific Build

Individual packages can be built using:
```bash
bun run --filter @paljs/[packag
```

</details>
