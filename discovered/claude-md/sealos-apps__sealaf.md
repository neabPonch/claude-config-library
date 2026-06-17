---
name: sealos-apps__sealaf
source: https://github.com/sealos-apps/sealaf/blob/37d5e116b724d3341b168b1d55293432c83e090a/CLAUDE.md
repo: sealos-apps/sealaf
kind: claude-md
stars: 29
last_pushed: 2026-05-25T10:24:31Z
license: unknown
score: 9
domains: [backend-api, web-frontend, monorepo]
tags: [nest-js, react, devops, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# sealos-apps/sealaf — claude-md

**Why it's worth keeping:** It provides explicit guidance on module structures, state management patterns (Zustand/Immer), and specific K8s-related local development commands like Telepresence.

**Summary:** A highly detailed technical specification that maps out the monorepo's architecture, development workflows, and coding patterns.

**Source credibility:** High; part of an active, specialized BaaS product repository.

**Recency:** Very recent; pushed 1 month ago.

**Source:** [sealos-apps/sealaf/CLAUDE.md](https://github.com/sealos-apps/sealaf/blob/37d5e116b724d3341b168b1d55293432c83e090a/CLAUDE.md) · 29★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Sealaf is a serverless function computing platform that deeply integrates [Laf](https://github.com/labring/laf) and [Sealos](https://github.com/labring/sealos). It provides Backend-as-a-Service (BaaS) capabilities including cloud functions, databases, storage, and billing management. The project is organized as a Lerna monorepo with two main packages:

- **server**: NestJS-based API server managing all backend operations
- **web**: React/Vite-based frontend providing the development interface

## Development Commands

### Root Level
```bash
# Install all dependencies for both server and web
npm install  # or: lerna exec npm install --parallel

# Lint all packages
npm run lint  # or: lerna run lint --parallel

# Lint staged files (pre-commit)
npm run lint-staged  # or: lerna exec --since HEAD --parallel -- lint-staged --no-stash

# Build all packages
npm run build  # or: lerna run build --parallel

# Watch mode for development
npm run watch  # or: lerna run watch --parallel

# Clean build artifacts
npm run clean:build
```

### Server (NestJS Backe
```

</details>
