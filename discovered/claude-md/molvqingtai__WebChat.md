---
name: molvqingtai__WebChat
source: https://github.com/molvqingtai/WebChat/blob/b5f1b0183a80ba089ad8e51f15f40dabd8089a50/CLAUDE.md
repo: molvqingtai/WebChat
kind: claude-md
stars: 2336
last_pushed: 2025-11-08T12:43:14Z
license: mit
score: 9
domains: [web-frontend, browser-extension, p2p]
tags: [DDD, WXT, WebRTC, Architecture]
curated: 2026-06-15
curated_by: config-scout
---

# molvqingtai/WebChat — claude-md

**Why it's worth keeping:** It explains complex business logic patterns (Remesh) with concrete code examples and details high-level synchronization behaviors that prevent breaking changes during refactoring.

**Summary:** Provides deep architectural context for a decentralized browser extension using Domain-Driven Design (DDD) and WebRTC.

**Source credibility:** High; a popular, active repository with significant stars.

**Recency:** Very recent; references modern technologies like React 19 and Tailwind v4.

**Source:** [molvqingtai/WebChat/CLAUDE.md](https://github.com/molvqingtai/WebChat/blob/b5f1b0183a80ba089ad8e51f15f40dabd8089a50/CLAUDE.md) · 2336★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

WebChat is a decentralized, serverless browser extension that enables anonymous P2P chat on any website using WebRTC. Built with WXT framework for cross-browser support (Chrome, Firefox, Edge).

## Key Technologies

- **WXT**: Browser extension framework (config: `wxt.config.ts`)
- **Remesh**: DDD framework for domain logic with true UI/logic separation (RxJS-based reactive state management)
- **Artico (@rtco/client)**: WebRTC P2P communication library (replaces previous trystero dependency)
- **React 19** with TypeScript
- **Tailwind CSS v4** with shadcn/ui components
- **Valibot**: Runtime schema validation

## Development Commands

```bash
# Development
npm run dev                  # Chrome dev mode with hot reload
npm run dev:firefox          # Firefox dev mode

# Type checking
npm run check                # Run TypeScript compiler without emitting files

# Linting
npm run lint                 # ESLint with auto-fix and cache

# Building
npm run build                # Production build for all browsers
npm run build:chrome         # Chrome production
```

</details>
