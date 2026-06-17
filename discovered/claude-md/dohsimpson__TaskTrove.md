---
name: dohsimpson__TaskTrove
source: https://github.com/dohsimpson/TaskTrove/blob/f5b9550096d6e6190dd12a82af487adcea66be06/CLAUDE.md
repo: dohsimpson/TaskTrove
kind: claude-md
stars: 1063
last_pushed: 2026-01-09T20:52:24Z
license: other
score: 9
domains: [web-frontend, monorepo, typescript]
tags: [turborepo, pnpm-catalog, jotai, nextjs]
curated: 2026-06-14
curated_by: config-scout
---

# dohsimpson/TaskTrove — claude-md

**Why it's worth keeping:** The specific instructions to use 'catalog:' prevent dependency drift in monorepos, while the mandatory planning protocol (PLAN-XYZ.md) establishes a high-quality development lifecycle for the agent.

**Summary:** Provides deep technical context for a complex Turborepo monorepo using JIT packages and strict pnpm catalog versioning. It explicitly outlines architectural patterns for Jotai state management and specific command execution workflows.

**Source credibility:** High; source is a popular open-source project with significant stars and recent updates.

**Recency:** Extremely current, referencing Next.js 15 and React 19.

**Source:** [dohsimpson/TaskTrove/CLAUDE.md](https://github.com/dohsimpson/TaskTrove/blob/f5b9550096d6e6190dd12a82af487adcea66be06/CLAUDE.md) · 1063★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

# Private Memory Files

- Read @~/.claude/memory/tasktrove-private-claude.md

## Table of Contents

- [Monorepo Structure](#monorepo-structure)
- [Essential Commands](#essential-commands)
- [Architecture Overview](#architecture-overview)
- [Type System](#type-system)
- [TypeScript Guidelines](#typescript-guidelines)
- [Components Guidelines](#components-guidelines)
- [API](#api)
- [Tools](#tools)
- [Troubleshooting](#troubleshooting)

## Monorepo Structure

**Architecture:** Turborepo monorepo with JIT (Just-In-Time) packages - TypeScript files imported directly without build step.

**Workspace Layout:**

```
TaskTrove-agent4/
├── apps/
│   └── web/              # Main Next.js application (was root before migration)
└── packages/
    ├── atoms/            # @tasktrove/atoms - Jotai state management
    ├── types/            # @tasktrove/types - Zod schemas & TypeScript types
    ├── constants/        # @tasktrove/constants - Shared constants
    ├── utils/            # @tasktrove/utils - Utility functions
    ├── eslint-config/    # @repo/eslint-config - Shared ESLin
```

</details>
