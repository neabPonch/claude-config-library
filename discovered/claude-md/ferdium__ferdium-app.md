---
name: ferdium__ferdium-app
source: https://github.com/ferdium/ferdium-app/blob/86291544daedf2a53a4386b02319ef5ec03b349a/CLAUDE.md
repo: ferdium/ferdium-app
kind: claude-md
stars: 4357
last_pushed: 2026-05-25T11:29:05Z
license: apache-2.0
score: 9
domains: [desktop-app, electron, frontend]
tags: [electron, react, mobx, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# ferdium/ferdium-app — claude-md

**Why it's worth keeping:** The explicit separation of Main vs Renderer processes and the tabular mapping of MobX stores provide essential structural context for complex event-driven apps.

**Summary:** Provides a deep architectural map of an Electron-based app, covering process models, state management stores, and dual API layers.

**Source credibility:** Highly credible; a large, well-maintained open-source project with high star count.

**Recency:** Very current, specifying modern Node.js and pnpm versions.

**Source:** [ferdium/ferdium-app/CLAUDE.md](https://github.com/ferdium/ferdium-app/blob/86291544daedf2a53a4386b02319ef5ec03b349a/CLAUDE.md) · 4357★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Ferdium is an Electron desktop app that aggregates messaging services (Slack, WhatsApp, Gmail, etc.) into a single window. It's a hard fork of Franz with no restrictions. Uses Electron + React + MobX + TypeScript with an embedded AdonisJS internal server.

## Essential Commands

```bash
pnpm install              # Install dependencies (requires Node 22.18.0, pnpm 10.14.0)
pnpm dev                  # Start esbuild in watch mode (serves on http://127.0.0.1:8080)
pnpm start                # Launch Electron with built app (run after dev or build)
pnpm start:all-dev        # Dev + Electron together (waits for dev server, then launches)
pnpm debug                # Same as start:all-dev but with DEBUG=Ferdium:* logging

pnpm test                 # Run Jest tests with coverage
pnpm test:watch           # Jest in watch mode
pnpm test -- --testPathPattern="test/helpers"  # Run specific test files

pnpm typecheck            # TypeScript type checking (tsc --noEmit)
pnpm lint                 # ESLint with zero warnings allowed (--max-warnings 0)
pnpm lint:fi
```

</details>
