---
name: akash-network__console
source: https://github.com/akash-network/console/blob/6d581d15854e7b20da4487d95eb0e55a302d09d4/CLAUDE.md
repo: akash-network/console
kind: claude-md
stars: 261
last_pushed: 2026-06-15T18:50:44Z
license: apache-2.0
score: 9
domains: [monorepo, backend-api, typescript]
tags: [npm-workspaces, testing-workflows, type-safety]
curated: 2026-06-15
curated_by: config-scout
---

# akash-network/console — claude-md

**Why it's worth keeping:** Includes high-density technical details like exact test execution patterns (including setup/teardown scripts) and a clear mapping of the monorepo's application vs package hierarchy.

**Summary:** Provides comprehensive context for a complex TypeScript monorepo, including specific command-line workflows for building, testing (unit, integration, functional), and linting.

**Source credibility:** High-quality open-source project within the Akash Network ecosystem with recent activity.

**Recency:** 

**Source:** [akash-network/console/CLAUDE.md](https://github.com/akash-network/console/blob/6d581d15854e7b20da4487d95eb0e55a302d09d4/CLAUDE.md) · 261★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Contribution Guidelines

This file aggregates all RFC (Request for Comments) contribution guidelines that have landed.

## General Project Description

This is a **monorepo** project using **npm workspaces**. All projects use **strict TypeScript** configuration (`"strict": true` in all `tsconfig.json` files), ensuring type safety across the entire codebase.

### Project Structure

The monorepo contains multiple applications and shared packages:

**Applications:**
- `apps/api` - Hono + OpenAPI REST API with tsyringe DI
- `apps/deploy-web` - Next.js frontend for deploying on Akash Network
- `apps/stats-web` - Next.js frontend for network statistics
- `apps/indexer` - Node.js blockchain indexer (Express, no DI)
- `apps/notifications` - NestJS service for handling notifications (NestJS built-in DI)
- `apps/log-collector` - Standalone log collector (vanilla Node.js + tsyringe)
- `apps/provider-proxy` - Hono service for proxying requests to providers (manual factory DI)
- `apps/provider-console` - Provider console application
- `apps/tx-signer` - Internal transaction signing service (Hono + tsyringe)

**Shared Packages:**
- `packages/database` - Database shared package (Drizzle ORM sch
```

</details>
