---
name: aarondfrancis__fast-paginate
source: https://github.com/aarondfrancis/fast-paginate/blob/2bed7d94644f237ababaeb8b3b6f4c9d1340354f/CLAUDE.md
repo: aarondfrancis/fast-paginate
kind: claude-md
stars: 1367
last_pushed: 2025-11-28T04:22:53Z
license: mit
score: 8
domains: [backend, php, laravel]
tags: [architecture-deep-dive, test-guidance]
curated: 2026-06-15
curated_by: config-scout
---

# aarondfrancis/fast-paginate — claude-md

**Why it's worth keeping:** Provides a step-by-step algorithmic walkthrough of the core logic and explicitly defines fallback conditions to prevent the agent from breaking edge cases.

**Summary:** Explains a specific deferred-join pagination strategy in Laravel, including command instructions for database-dependent testing.

**Source credibility:** High; based on a popular (1.3k+ stars) specialized Laravel package.

**Recency:** 

**Source:** [aarondfrancis/fast-paginate/CLAUDE.md](https://github.com/aarondfrancis/fast-paginate/blob/2bed7d94644f237ababaeb8b3b6f4c9d1340354f/CLAUDE.md) · 1367★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Fast Paginate is a Laravel package that provides an optimized `limit`/`offset` pagination method using a "deferred join" technique. Instead of fetching full rows during pagination, it first retrieves only primary keys in an optimized subquery, then fetches full records for those specific IDs. This significantly improves performance on large datasets.

## Commands

**Run all tests:**
```bash
./vendor/bin/phpunit
```

**Run a specific test file:**
```bash
./vendor/bin/phpunit tests/Integration/BuilderTest.php
```

**Run a specific test method:**
```bash
./vendor/bin/phpunit --filter basic_test
```

**Note:** Tests require a MySQL database (8.4+). Configure via environment variables or `phpunit.xml`:
- DB_DATABASE=fast_paginate
- DB_USERNAME=test
- DB_PASSWORD=root

## Architecture

The package registers macros on Laravel's Eloquent Builder and Relation classes via `FastPaginateProvider`:

- **`FastPaginate`** (`src/FastPaginate.php`): Core pagination logic. Implements `fastPaginate()` and `simpleFastPaginate()` methods that:
  1. Clone the query an
```

</details>
