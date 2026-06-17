---
name: kunkunsh__kunkun
source: https://github.com/kunkunsh/kunkun/blob/cb8af4930dfbd1ca9f252e73475faa6416e20428/CLAUDE.md
repo: kunkunsh/kunkun
kind: claude-md
stars: 1283
last_pushed: 2026-02-10T14:50:36Z
license: other
score: 9
domains: [desktop-apps, monorepos, rust]
tags: [tauri, sveltekit, monorepo, pnpm]
curated: 2026-06-15
curated_by: config-scout
---

# kunkunsh/kunkun — claude-md

**Why it's worth keeping:** Uses highly specific filtered commands (pnpm --filter) and explicit directory mapping which is essential for preventing an AI from getting lost in large-scale monorepos.

**Summary:** A comprehensive guide for a complex Tauri/SvelteKit monorepo that maps architecture to specific development workflows.

**Source credibility:** High; a popular open-source project with significant stars and recent maintenance activity.

**Recency:** Very current, utilizing modern versions of Node, SvelteKit, and Tauri.

**Source:** [kunkunsh/kunkun/CLAUDE.md](https://github.com/kunkunsh/kunkun/blob/cb8af4930dfbd1ca9f252e73475faa6416e20428/CLAUDE.md) · 1283★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Kunkun is a cross-platform desktop application built with Tauri (Rust backend) and SvelteKit (frontend). It's an extensible launcher/utility app that supports custom extensions developed in various web frameworks.

## Development Commands

### Essential Commands
- `pnpm install` - Install all dependencies
- `pnpm build` - Build all packages and submodules
- `pnpm dev` - Start development servers for all packages
- `pnpm lint` - Run linting across all packages
- `pnpm test` - Run tests across all packages
- `pnpm check-types` - Run TypeScript type checking
- `pnpm format` - Format code with Prettier

### Desktop App Specific
- `pnpm --filter @kksh/desktop tauri dev` - Run desktop app in development mode
- `cd apps/desktop && pnpm tauri dev` - Alternative way to run desktop app
- `cd apps/desktop && pnpm tauri build` - Build desktop app for production

### Prerequisites for Development
- Node.js ≥22
- pnpm 10.7.0+ (package manager)
- Rust (for Tauri backend)
- Bun, Deno (for various tools)
- protobuf (`brew install protobuf` on macOS)
- cmake (`brew instal
```

</details>
