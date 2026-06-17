---
name: neilsarkar__labs
source: https://github.com/neilsarkar/labs/blob/6d606b05ddeba2a2f3ca2ce508586e5b8e63b9e3/CLAUDE.md
repo: neilsarkar/labs
kind: claude-md
stars: 0
last_pushed: 2026-01-16T20:19:08Z
license: unknown
score: 8
domains: [backend-api, systems-programming, web-runtime]
tags: [bun, zig, wasm, monorepo, tooling-migration]
curated: 2026-06-16
curated_by: config-scout
---

# neilsarkar/labs — claude-md

**Why it's worth keeping:** The 'Use X instead of Y' pattern is highly effective at overriding LLM biases toward standard Node.js/npm patterns. It also defines specific build/test commands necessary for navigating the monorepo.

**Summary:** Provides explicit toolchain preferences and API replacements for a Bun-centric development environment.

**Source credibility:** Personal experimental repository with low social proof but high technical specificity.

**Recency:** Highly current; reflects modern Bun development workflows.

**Source:** [neilsarkar/labs/CLAUDE.md](https://github.com/neilsarkar/labs/blob/6d606b05ddeba2a2f3ca2ce508586e5b8e63b9e3/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Experimental monorepo exploring Bun, Zig, WebAssembly, and WebRTC technologies. Organized as a Bun workspace with independent spike projects in `spikes/`.

## Commands

```bash
bun install              # Install all dependencies
bun test                 # Run all tests
bun run build            # Build all spikes
bun run ci:tsc           # TypeScript type checking across all spikes
bun run dev              # Start dev servers for all spikes
```

For Zig projects (aoc25, memory, zgpu):
```bash
zig build                # Build
zig build run            # Build and run
zig build test           # Run tests
```

## Use Bun Instead of Node.js

- Use `bun <file>` instead of `node` or `ts-node`
- Use `bun test` instead of `jest` or `vitest`
- Use `bun install` instead of `npm/yarn/pnpm install`
- Bun automatically loads `.env` files

### Bun APIs

- `Bun.serve()` for HTTP/WebSocket servers (not express)
- `bun:sqlite` for SQLite (not better-sqlite3)
- `Bun.file` over `node:fs` readFile/writeFile
- `Bun.$\`cmd\`` instead of execa
- Built-in `WebSocket` (not ws pack
```

</details>
