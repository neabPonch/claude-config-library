---
name: statamic__eloquent-driver
source: https://github.com/statamic/eloquent-driver/blob/a7c01cc86ede81f7fa4d1c579afddf59c5276d79/CLAUDE.md
repo: statamic/eloquent-driver
kind: claude-md
stars: 126
last_pushed: 2026-06-11T08:10:44Z
license: mit
score: 9
domains: [php, backend]
tags: [statamic, eloquent, database-driver]
curated: 2026-06-16
curated_by: config-scout
---

# statamic/eloquent-driver — claude-md

**Why it's worth keeping:** It details critical architectural patterns like model inheritance and specific trait usage (QueriesJsonColumns), plus vital test setup nuances that prevent environment mismatches.

**Summary:** Provides context for a Statamic driver that swaps flat-file storage for Eloquent/database logic. It includes clear command shortcuts and structural guidance.

**Source credibility:** High; based on a specialized, well-maintained Statamic extension.

**Recency:** Current; reflects modern PHP/Laravel development standards.

**Source:** [statamic/eloquent-driver/CLAUDE.md](https://github.com/statamic/eloquent-driver/blob/a7c01cc86ede81f7fa4d1c579afddf59c5276d79/CLAUDE.md) · 126★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

A Statamic addon (`statamic/eloquent-driver`) that replaces Statamic's flat-file Stache storage with Eloquent/database-backed repositories. Each Statamic data type (entries, collections, taxonomies, etc.) can be independently switched between `file` and `eloquent` drivers via config.

## Commands

```bash
# Run all tests
./vendor/bin/phpunit

# Run a single test file
./vendor/bin/phpunit tests/Entries/EntryTest.php

# Run a specific test method
./vendor/bin/phpunit --filter testMethodName

# Lint
./vendor/bin/pint
```

Tests use SQLite in-memory by default (configured in `phpunit.xml.dist`).

## Architecture

### Driver registration pattern

`ServiceProvider.php` is the core file. Each data type has a `register*()` method that:
1. Always binds the model class to the container (even when driver is `file`)
2. Conditionally registers the Eloquent repository and excludes the Stache store only when `driver === 'eloquent'`

Each repository replaces a Statamic contract (e.g. `EntryRepositoryContract`) with an Eloquent implementation that extends the corresp
```

</details>
