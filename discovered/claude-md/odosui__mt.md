---
name: odosui__mt
source: https://github.com/odosui/mt/blob/9d2c18ef4eb725fcada4a2d71f504e294e7aa1ce/CLAUDE.md
repo: odosui/mt
kind: claude-md
stars: 33
last_pushed: 2026-06-14T08:25:09Z
license: unknown
score: 8
domains: [fullstack, web-development, monorepo]
tags: [react, express, typescript, monorepo]
curated: 2026-06-14
curated_by: config-scout
---

# odosui/mt — claude-md

**Why it's worth keeping:** Excellent categorization of lifecycle commands (setup/dev/test) and explicit detail on project-specific technical constraints like strict TypeScript configurations.

**Summary:** A comprehensive guide for a full-stack monorepo featuring detailed command instructions and architectural boundaries.

**Source credibility:** Active repository with recent maintenance; demonstrates real-world application usage.

**Recency:** Highly current, specifically mentioning modern technologies like React 19.

**Source:** [odosui/mt/CLAUDE.md](https://github.com/odosui/mt/blob/9d2c18ef4eb725fcada4a2d71f504e294e7aa1ce/CLAUDE.md) · 33★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**mt** is a knowledge management app with spaced repetition. Notes are markdown files stored on the local filesystem (default `~/mt`). The app has a React SPA frontend and an Express API backend, organized as a monorepo with `client/` and `server/` subdirectories.

The project is spec-driven approach with all the features described in 'features.md' being the single source of truth for everything we build.

## Commands

### Setup

```bash
npm install && npm run install-client && npm run install-server
```

### Development

```bash
npm run dev              # Starts both client (Vite :5173) and server (nodemon :3000) concurrently
npm run dev --prefix client   # Client only
npm run dev --prefix server   # Server only
```

### Build & Start

```bash
npm run build            # Builds both client and server
npm run start            # Production start (NODE_ENV=production required)
```

### Type Checking & Linting

```bash
npm run check-types --prefix client
npm run check-types --prefix server
npm run lint --prefix client        # oxlint
```

### Tests (
```

</details>
