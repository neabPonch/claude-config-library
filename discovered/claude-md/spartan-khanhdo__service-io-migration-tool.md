---
name: spartan-khanhdo__service-io-migration-tool
source: https://github.com/spartan-khanhdo/service-io-migration-tool/blob/a7fd72d8bf7f120c3cb7c640713df64fb5d44723/CLAUDE.md
repo: spartan-khanhdo/service-io-migration-tool
kind: claude-md
stars: 0
last_pushed: 2026-04-12T10:39:01Z
license: unknown
score: 9
domains: [data-migration, backend-engineering, database-administration]
tags: [typescript, postgresql, migration, etl]
curated: 2026-06-17
curated_by: config-scout
---

# spartan-khanhdo/service-io-migration-tool — claude-md

**Why it's worth keeping:** It provides explicit transformation logic (ID mappings, type conversions) and strict operational constraints that are essential for an AI to perform risk-sensitive data tasks.

**Summary:** A high-density technical specification for a complex data migration tool involving schema transitions between PHP/Laravel and Kotlin/Exposed.

**Source credibility:** Low public social proof (0 stars), but demonstrates high professional engineering depth through specific schema alignment details.

**Recency:** Highly current; mentions modern tooling like pnpm@10.25.0 and tsx.

**Source:** [spartan-khanhdo/service-io-migration-tool/CLAUDE.md](https://github.com/spartan-khanhdo/service-io-migration-tool/blob/a7fd72d8bf7f120c3cb7c640713df64fb5d44723/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Service IO Migration Tool

## Overview
Migration tool to transfer data from the old PHP/Laravel database (`service-loanbud-io`) to the new Kotlin/Exposed database (`service-io`).

**Status**: Updated for Flyway 000-065. Needs re-testing after schema alignment migrations 042-065.

## Tech Stack
- **Runtime**: Node.js
- **Language**: TypeScript (strict mode)
- **Package Manager**: pnpm@10.25.0
- **Database Client**: `pg` (node-postgres)
- **Build**: tsx (for running TS directly)

## Project Structure
```
src/
├── index.ts                 # Entry point - orchestrates phases
├── config/
│   ├── database.ts          # Old DB + New DB connection pool config
│   └── ssh-tunnel.ts        # Optional SSH tunnel for AWS RDS
├── parser/
│   ├── composite-type.ts    # Parse PostgreSQL composite types (table_item_type, state_type, naics_type)
│   └── polymorphic.ts       # Transform model_type values (App\Models\X → x)
├── mapping/
│   └── id-mapping-store.ts  # In-memory old_id → new_uuid mapping (roles, permissions, media)
├── phases/
│   ├── phase-0-validate.ts  # Pre-flight checks (DB connectivity, table existence, Flyway state)
│   ├── phase-1/             # Reference data: states, counti
```

</details>
