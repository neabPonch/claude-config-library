---
name: Stellar-Atlas__StellarAtlas
source: https://github.com/Stellar-Atlas/StellarAtlas/blob/2a23ba0e92fcb577678b229fb5239d3596403dd3/CLAUDE.md
repo: Stellar-Atlas/StellarAtlas
kind: claude-md
stars: 1
last_pushed: 2026-05-30T00:55:01Z
license: mit
score: 8
domains: [backend-api, monorepo, blockchain]
tags: [typescript, ddd, pnpm, node-js]
curated: 2026-06-15
curated_by: config-scout
---

# Stellar-Atlas/StellarAtlas — claude-md

**Why it's worth keeping:** It explicitly defines code patterns (Use Cases/Infrastructure) and dependency injection styles, which prevents the AI from deviating from the project's established architecture.

**Summary:** A highly structured guide for a complex TypeScript monorepo that details command shorthands, architectural patterns (DDD), and environment configurations.

**Source credibility:** Single-star niche repo; content appears to be a high-quality internal developer guide.

**Recency:** Very current, referencing Node 22 and pnpm 10.

**Source:** [Stellar-Atlas/StellarAtlas/CLAUDE.md](https://github.com/Stellar-Atlas/StellarAtlas/blob/2a23ba0e92fcb577678b229fb5239d3596403dd3/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Essential Commands

### Development
- `pnpm dev` - Start development environment (backend API on :3000, frontend on :5173)
- `pnpm build:ts` - Compile TypeScript for all apps/packages
- `pnpm build` - Full build including frontend
- `pnpm lint` - Run ESLint across entire monorepo

### Testing  
- `pnpm test:unit` or `pnpm tu` - Run unit tests
- `pnpm test:integration` or `pnpm ti` - Run integration tests (requires PostgreSQL)
- `pnpm test:all` - Run all tests
- Specific test suites: `pnpm test:unit:frontend`, `pnpm test:unit:backend`, `pnpm test:unit:crawler`, etc.

### Production Services
- `pnpm start:api` - Start backend REST API
- `pnpm start:frontend` - Start frontend server
- `pnpm start:scan-network` - Start network scanning (args: loop, dry-run)
- `pnpm start:scan-history` - Start history archive scanning (args: persist, loop)

## Architecture Overview

**StellarAtlas** is a monitoring and analytics platform for the Stellar network. This monorepo follows clean architecture principles with domain-driven design.

### Core Applications

**Backend** (`apps/bac
```

</details>
