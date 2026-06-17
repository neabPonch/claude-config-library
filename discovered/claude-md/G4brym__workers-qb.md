---
name: G4brym__workers-qb
source: https://github.com/G4brym/workers-qb/blob/7a214d1e2016989bb6775ea991d730790ac6aba0/CLAUDE.md
repo: G4brym/workers-qb
kind: claude-md
stars: 394
last_pushed: 2026-04-13T17:41:16Z
license: mit
score: 9
domains: [backend-api, database-tools, cloud-infrastructure]
tags: [typescript, cloudflare-workers, sql-builder, architecture-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# G4brym/workers-qb — claude-md

**Why it's worth keeping:** The 'Critical' section uses explicit 'Correct/Wrong' code examples to prevent the model from incorrectly applying `await` to synchronous methods. It also maps out the relationship between the type system and actual runtime execution behavior.

**Summary:** Provides structural architecture and critical behavioral constraints for a specialized query builder. It specifically addresses the nuance of synchronous vs. asynchronous operations to prevent logic errors.

**Source credibility:** High; 394 stars indicates a widely-used specialized tool with active maintenance.

**Recency:** Current; utilizes modern Vitest patterns and reflects contemporary Cloudflare Workers development paradigms.

**Source:** [G4brym/workers-qb/CLAUDE.md](https://github.com/G4brym/workers-qb/blob/7a214d1e2016989bb6775ea991d730790ac6aba0/CLAUDE.md) · 394★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build Commands

```bash
npm run build        # Build library (tsup → dist/)
npm run lint         # Lint and auto-fix with Biome
npm run test         # Run all tests (requires npm install first)
npm run test:types   # Type-check tests only

# Run a single test file
npx vitest run --root tests tests/unit/select.test.ts

# Run tests matching a pattern
npx vitest run --root tests -t "insert"
```

## Architecture

**workers-qb** is a zero-dependency query builder for Cloudflare Workers with three database implementations:

### Database Classes (extend `QueryBuilder`)
- **`D1QB`** (`src/databases/d1.ts`) - Cloudflare D1, **async** operations
- **`DOQB`** (`src/databases/do.ts`) - Durable Objects SQLite, **sync** operations
- **`PGQB`** (`src/databases/pg.ts`) - PostgreSQL via node-postgres, **async** operations

### Core Components
- **`QueryBuilder`** (`src/builder.ts`) - Abstract base class with SQL generation (`_select`, `_insert`, `_update`, `_delete`) and query methods (`fetchOne`, `fetchAll`, `insert`, `update`, `delete`, `raw`)
- **`SelectBuilder`** (`src/modular
```

</details>
