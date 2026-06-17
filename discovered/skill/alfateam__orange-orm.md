---
name: alfateam__orange-orm
source: https://github.com/alfateam/orange-orm/blob/47501636fa2ba94408d14c7056ed5b859e8394ef/SKILL.md
repo: alfateam/orange-orm
kind: skill
stars: 1001
last_pushed: 2026-06-14T12:19:50Z
license: isc
score: 9
domains: [backend, database-orm, typescript]
tags: [orm, typescript, active-record, sql]
curated: 2026-06-15
curated_by: config-scout
---

# alfateam/orange-orm — skill

**Why it's worth keeping:** Uses highly specific code patterns (like .notNullExceptInsert() and fetching strategies) that teach an agent exactly how to handle complex database constraints and relations without ambiguity.

**Summary:** Provides high-density API reference and pattern examples for the Orange ORM, covering schema mapping, connections, and CRUD operations.

**Source credibility:** High; 1k+ stars indicates a well-established, community-vetted tool.

**Recency:** Very current; repository shows active maintenance within the last month.

**Source:** [alfateam/orange-orm/SKILL.md](https://github.com/alfateam/orange-orm/blob/47501636fa2ba94408d14c7056ed5b859e8394ef/SKILL.md) · 1001★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Orange ORM — Skills & Reference

> Authoritative reference for [context7.com](https://context7.com/alfateam/orange-orm) MCP consumption.
> Orange ORM is the ultimate Object Relational Mapper for Node.js, Bun, and Deno.
> It uses the **Active Record Pattern** with full TypeScript IntelliSense — no code generation required.
> Supports: PostgreSQL, SQLite, MySQL, MS SQL, Oracle, SAP ASE, PGlite, Cloudflare D1.
> Works in the browser via Express/Hono adapters.

## Repository maintenance note

- Treat `dist/index.mjs` and `dist/index.browser.mjs` as generated build output from the build command, not as source files to review or edit directly unless the task explicitly targets build artifacts.

---

## Table of Contents

1. [Defining a Model (Table Mapping)](#defining-a-model-table-mapping)
2. [Connecting to a Database](#connecting-to-a-database)
3. [Inserting Rows](#inserting-rows)
4. [Fetching Rows](#fetching-rows)
5. [Filtering (where)](#filtering-where)
6. [Ordering, Limit, Offset](#ordering-limit-offset)
7. [Updating Rows (saveChanges)](#updating-rows-savechanges)
8. [Deleting Rows](#deleting-rows)
9. [Relationships (hasMany, hasOne, references)](#relationships-hasmany-hasone-refe
```

</details>
