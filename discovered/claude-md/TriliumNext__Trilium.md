---
name: TriliumNext__Trilium
source: https://github.com/TriliumNext/Trilium/blob/655e5123b74247a8402193c256448fac76f32669/CLAUDE.md
repo: TriliumNext/Trilium
kind: claude-md
stars: 36461
last_pushed: 2026-06-15T17:16:25Z
license: agpl-3.0
score: 9
domains: [fullstack, monorepo, architecture-guidance]
tags: [monorepo, typescript, cache-layers, architectural-constraints]
curated: 2026-06-15
curated_by: config-scout
---

# TriliumNext/Trilium — claude-md

**Why it's worth keeping:** Excellent use of 'negative constraints' (e.g., prohibiting direct DB writes) and detailed explanation of critical cache layers to prevent state desynchronization.

**Summary:** Comprehensive technical manual that combines development workflows with strict architectural guardrails for a complex monorepo.

**Source credibility:** Highly credible; high-star, actively maintained project.

**Recency:** 

**Source:** [TriliumNext/Trilium/CLAUDE.md](https://github.com/TriliumNext/Trilium/blob/655e5123b74247a8402193c256448fac76f32669/CLAUDE.md) · 36461★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

> **Note**: When updating this file, also update `.github/copilot-instructions.md` to keep both AI coding assistants in sync.

## Overview

Trilium Notes is a hierarchical note-taking application with synchronization, scripting, and rich text editing. TypeScript monorepo using pnpm with multiple apps and shared packages.

## Development Commands

```bash
# Setup
corepack enable && pnpm install

# Run
pnpm server:start              # Dev server at http://localhost:8080
pnpm desktop:start             # Electron dev app
pnpm standalone:start          # Standalone client dev

# Build
pnpm client:build              # Frontend
pnpm server:build              # Backend
pnpm desktop:build             # Electron

# Test
pnpm test:all                  # All tests (parallel + sequential)
pnpm test:parallel             # Client + most package tests
pnpm test:sequential           # Server (shared DB) + browser-mode tests (ckeditor5, ckeditor5-mermaid, ckeditor5-math)
pnpm --filter server test      # Single package tests
pnpm coverage                  # Coverage reports

# Lint & F
```

</details>
