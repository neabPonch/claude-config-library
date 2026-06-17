---
name: rainbow-me__rainbowkit
source: https://github.com/rainbow-me/rainbowkit/blob/03360ee924cfa6af13ff1d623b356bf5a170348e/CLAUDE.md
repo: rainbow-me/rainbowkit
kind: claude-md
stars: 2822
last_pushed: 2026-05-12T08:57:32Z
license: mit
score: 10
domains: [web-frontend, monorepo]
tags: [monorepo, git-workflow]
curated: 2026-06-14
curated_by: config-scout
---

# rainbow-me/rainbowkit — claude-md

**Why it's worth keeping:** Includes highly specific operational instructions for Git tools (Graphite/gt) and detailed build process explanations that prevent AI-driven build failures.

**Summary:** A comprehensive guide for navigating a complex monorepo including specific architecture details and specialized tool workflows.

**Source credibility:** High; popular, well-maintained industry library.

**Recency:** Very current, using modern Node and Biome toolchains.

**Source:** [rainbow-me/rainbowkit/CLAUDE.md](https://github.com/rainbow-me/rainbowkit/blob/03360ee924cfa6af13ff1d623b356bf5a170348e/CLAUDE.md) · 2822★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Monorepo Structure

RainbowKit is a pnpm monorepo containing multiple packages:

- **`packages/rainbowkit`** - Core library: React components and hooks for wallet connection UI
- **`packages/rainbow-button`** - Standalone rainbow button component
- **`packages/rainbowkit-siwe-next-auth`** - Sign-In with Ethereum integration with NextAuth.js
- **`packages/create-rainbowkit`** - CLI tool for scaffolding new RainbowKit projects
- **`packages/example`** - Development example app (runs on localhost:3000)
- **`site`** - Documentation site (runs on localhost:3001)
- **`examples/`** - Additional example integrations (Next.js, Vite, Remix, etc.)

## Development Commands

### Setup
```bash
pnpm install  # Install dependencies and generate type definitions from root
```

### Development
```bash
pnpm dev                      # Run example app + site (localhost:3000 and :3001)
pnpm dev:lib                  # Watch and rebuild library packages only
pnpm dev:example              # Run lib + example app only
pnpm dev:site                 # Run lib + docs site only
pnpm dev:cli
```

</details>
