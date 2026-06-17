---
name: KevinEdry__nestjs-trpc
source: https://github.com/KevinEdry/nestjs-trpc/blob/6eaf1cd0ff49160c11ce0bf45a90a6c892c17f41/CLAUDE.md
repo: KevinEdry/nestjs-trpc
kind: claude-md
stars: 332
last_pushed: 2026-02-26T18:02:24Z
license: mit
score: 9
domains: [backend-api, typescript]
tags: [architecture, codegen, nestjs, monorepo]
curated: 2026-06-15
curated_by: config-scout
---

# KevinEdry/nestjs-trpc — claude-md

**Why it's worth keeping:** It includes high-value 'Implementation Notes' that warn about fragile patterns like stack-trace-based path resolution and the critical need to keep Codegen in sync with Runtime logic.

**Summary:** Provides a deep architectural breakdown of the library's decorator-based, reflection-driven system.

**Source credibility:** High; a well-regarded open-source library with significant star count and recent activity.

**Recency:** Current; uses modern tooling like Bun and updated TypeScript patterns.

**Source:** [KevinEdry/nestjs-trpc/CLAUDE.md](https://github.com/KevinEdry/nestjs-trpc/blob/6eaf1cd0ff49160c11ce0bf45a90a6c892c17f41/CLAUDE.md) · 332★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**NestJS tRPC** is a library that integrates tRPC into the NestJS framework using an opinionated, decorator-based approach that aligns with NestJS conventions. It provides end-to-end typesafety for APIs with automatic AppRouter generation and full dependency injection support.

## Development Commands

### Build & Development
```bash
# Build all packages (uses TypeScript project references)
bun run build

# Build nestjs-trpc package only
cd packages/nestjs-trpc && bun run build

# Watch mode for development
cd packages/nestjs-trpc && bun run start:dev

# Debug with Node inspector
cd packages/nestjs-trpc && bun run debug:dev

# Clean build artifacts
bun run clean
```

### Testing
```bash
# Run all tests (workspace-wide)
bun test

# Run tests for nestjs-trpc package only
cd packages/nestjs-trpc && bun test

# Run tests with coverage
cd packages/nestjs-trpc && bun test --coverage

# Run related tests for changed files (used by lint-staged)
bun test --bail --findRelatedTests <file>
```

### Linting & Formatting
```bash
# Lint and auto-fix
bun run lin
```

</details>
