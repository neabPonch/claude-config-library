---
name: Mathews-Tom__armory__skill
source: https://github.com/Mathews-Tom/armory/blob/789d0c83a89f02a02b1addcdd56a270b4b72dac7/skills/sql-optimizer/SKILL.md
repo: Mathews-Tom/armory
kind: skill
stars: 250
last_pushed: 2026-06-05T20:59:23Z
license: mit
score: 9
domains: [database, backend, performance]
tags: [sql, optimization, dba, performance-tuning]
curated: 2026-06-16
curated_by: config-scout
---

# Mathews-Tom/armory — skill

**Why it's worth keeping:** The tiered optimization modes (quick/standard/deep) and the 'Calibration Rules' that enforce professional DBA best practices like index write overhead and statistical validation.

**Summary:** Provides a multi-phase, systematic workflow for database performance analysis using EXPLAIN plans and anti-pattern detection.

**Source credibility:** High; 250 stars and very recent updates indicate a high-quality, community-vetted production repository.

**Recency:** 

**Source:** [Mathews-Tom/armory/skills/sql-optimizer/SKILL.md](https://github.com/Mathews-Tom/armory/blob/789d0c83a89f02a02b1addcdd56a270b4b72dac7/skills/sql-optimizer/SKILL.md) · 250★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: sql-optimizer
description: 'Analyzes SQL queries for missing indexes, N+1 patterns, suboptimal joins, and full table scans. Interprets EXPLAIN, detects anti-patterns, rewrites queries. Triggers on: "optimize this query", "slow query", "add indexes", "explain plan", "N+1 query", "why is this query slow".'
metadata:
  version: 1.1.1
  category: data
  tags: [sql, performance, database, optimization]
  difficulty: intermediate
  phase: build
---

# SQL Optimizer

Systematic SQL performance analysis: parse query structure, interpret EXPLAIN plans,
detect anti-patterns (N+1, full scans, cartesian joins), recommend indexes, and rewrite
queries — with explanations of WHY each change improves performance, not just WHAT changed.

## Reference Files

| File                              | Contents                                                                  | Load When                          |
| --------------------------------- | ------------------------------------------------------------------------- | ---------------------------------- |
| `references/anti-patterns.md`     | Common SQL anti-patterns with detection rules and fixes                   | Always
```

</details>
