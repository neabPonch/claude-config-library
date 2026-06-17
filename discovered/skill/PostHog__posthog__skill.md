---
name: PostHog__posthog__skill
source: https://github.com/PostHog/posthog/blob/1746f9a813fa25adf47ed83193231ff7e2773105/.agents/skills/optimizing-clickhouse-and-hogql-queries/SKILL.md
repo: PostHog/posthog
kind: skill
stars: 35053
last_pushed: 2026-06-16T05:12:48Z
license: other
score: 9
domains: [database, performance-optimization, backend-engineering]
tags: [clickhouse, hogql, query-optimization, troubleshooting]
curated: 2026-06-16
curated_by: config-scout
---

# PostHog/posthog — skill

**Why it's worth keeping:** It provides a superior investigative mental model: tracing high-level abstractions down to raw SQL execution. It also includes specific 'search patterns' (grep targets) to catch hidden duplication between frontend and backend layers.

**Summary:** A highly specialized playbook for identifying and optimizing ClickHouse and HogQL queries across a complex monorepo.

**Source credibility:** Extremely high; sourced from PostHog, an industry-standard data platform with a highly mature engineering culture.

**Recency:** Very current; reflects modern monorepo ownership/triage patterns used in large-scale distributed systems.

**Source:** [PostHog/posthog/.agents/skills/optimizing-clickhouse-and-hogql-queries/SKILL.md](https://github.com/PostHog/posthog/blob/1746f9a813fa25adf47ed83193231ff7e2773105/.agents/skills/optimizing-clickhouse-and-hogql-queries/SKILL.md) · 35053★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: optimizing-clickhouse-and-hogql-queries
description: Workflow for optimizing ClickHouse and HogQL queries. Use when a HogQL query, query runner, insight, or report is too slow; when a hand-written ClickHouse query (via `sync_execute` or in a migration) is too slow; when ClickHouse times out or hits memory limits; when investigating a slow `system.query_log` row; or when reviewing a proposed HogQL printer change for performance. Covers extracting the ClickHouse SQL (for HogQL queries), common smells (`FROM ... FINAL`, `JSONExtract` over properties, missing skip indexes, self-joins, CTE blow-up), measuring against a real cluster, and applying the fix at the right layer (printer, query runner, or ClickHouse migration). Does NOT cover Postgres / Django ORM / app-database queries; those need pganalyze and the Postgres section of `query-performance-optimization.md`, not this skill.
---

# Optimizing ClickHouse and HogQL queries

**Scope:** this skill optimizes **ClickHouse queries** and **HogQL queries** (which compile to ClickHouse). It does **not** optimize Postgres / Django ORM / app-database queries. If the slow query you're holding is a `Model.objects.filter(...)` or any o
```

</details>
