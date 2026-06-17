---
name: marktext__marktext
source: https://github.com/marktext/marktext/blob/3eaefce6fb9a0b49443e951dd4def77191042bf2/CLAUDE.md
repo: marktext/marktext
kind: claude-md
stars: 57363
last_pushed: 2026-06-15T01:32:19Z
license: mit
score: 9
domains: [desktop-app, monorepo, frontend]
tags: [pnpm-workspace, electron, vue3, navigation-guide]
curated: 2026-06-15
curated_by: config-scout
---

# marktext/marktext — claude-md

**Why it's worth keeping:** The detailed mapping of the monorepo's internal plumbing—specifically how root scripts proxy to specific packages—is essential for AI tool-use. It also provides exact versioning (e.g., TS 5.9) to prevent API incompatibility hallucinations.

**Summary:** Provides a comprehensive technical map of a complex pnpm monorepo, detailing technology versions and package relationships.

**Source credibility:** Highly credible: high-star, active open-source project with detailed documentation.

**Recency:** Very current; mentions cutting-edge versions like TypeScript 5.9 and pnpm 10.

**Source:** [marktext/marktext/CLAUDE.md](https://github.com/marktext/marktext/blob/3eaefce6fb9a0b49443e951dd4def77191042bf2/CLAUDE.md) · 57363★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

# MarkText

## Project Overview

MarkText is a WYSIWYG markdown editor built on Electron + Vue 3. It supports CommonMark, GitHub Flavored Markdown, math (KaTeX), Mermaid diagrams, PlantUML, and multiple editing modes (focus, typewriter, source-code).

- **Version**: see `package.json`
- **License**: MIT
- **Repository**: https://github.com/marktext/marktext

## Tech Stack

| Layer | Technology |
|---|---|
| Language | TypeScript 5.9 (strict mode) — `packages/muyajs/` retained as JS via ambient shim |
| Desktop shell | Electron 42 |
| Build system | electron-vite 5 |
| Packaging | electron-builder 26 |
| Frontend framework | Vue 3 |
| State management | Pinia 3 |
| Routing | Vue Router 4 |
| UI library | Element Plus |
| Unit tests | Vitest 4 |
| E2E tests | Playwright |
| Package manager | pnpm >=10 workspace (`packageManager: pnpm@10.33.4`) |
| Repo layout | pnpm monorepo — see Directory Structure |
| Node.js minimum | >=20.19.0 (PR CI: Node 22.21.1 · release CI: Node 24.14.1) |

## Directory Structure

This is a pnpm workspace. Three packages live under `packages/`
```

</details>
