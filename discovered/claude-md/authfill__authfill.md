---
name: authfill__authfill
source: https://github.com/authfill/authfill/blob/2a6fb715bdc1538887c5019085644f717159b4df/CLAUDE.md
repo: authfill/authfill
kind: claude-md
stars: 45
last_pushed: 2026-03-16T18:49:50Z
license: gpl-3.0
score: 8
domains: [web-extension, monorepo, fullstack]
tags: [pnpm, turbo, architecture-map]
curated: 2026-06-15
curated_by: config-scout
---

# authfill/authfill — claude-md

**Why it's worth keeping:** Specifically documents inter-app communication patterns (message passing vs WebSockets) and platform-specific build commands to prevent AI hallucinations in mono-repo workflows.

**Summary:** Provides essential architectural context for a complex pnpm monorepo and explains how different parts of the extension interact.

**Source credibility:** A specialized project with recent, high-quality maintenance and modern dependencies.

**Recency:** Extremely current, utilizing React 19 and Node 22.

**Source:** [authfill/authfill/CLAUDE.md](https://github.com/authfill/authfill/blob/2a6fb715bdc1538887c5019085644f717159b4df/CLAUDE.md) · 45★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

AuthFill is a browser extension for one-click email verification. It connects to email providers via IMAP to fetch verification codes/links automatically.

## Common Commands

```bash
# Development (starts all apps via Turbo)
pnpm run dev

# Build all packages
pnpm run build

# Lint all packages
pnpm run lint

# Format code
pnpm run format

# Build extension for specific browser
pnpm --filter extension build:chrome
pnpm --filter extension build:firefox
pnpm --filter extension build:edge
pnpm --filter extension build:opera

# Deploy proxy to Cloudflare Workers
pnpm --filter proxy deploy
```

## Architecture

This is a pnpm monorepo managed with Turbo. Structure:

```
apps/
  extension/    # Browser extension (React popup + background service worker)
  proxy/        # Cloudflare Worker - IMAP proxy via WebSocket
  web/          # Landing page (TanStack Start)
packages/
  ui/           # Shared Radix UI components
  hooks/        # Shared React hooks
  eslint/       # Shared ESLint config
  typescript/   # Shared TypeScript config
```

### Extension
```

</details>
