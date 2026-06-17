---
name: baserow__baserow__skill
source: https://github.com/baserow/baserow/blob/b8c8d51a46dfd845f556c52266121374a3404696/.agents/skills/silk-profiler/SKILL.md
repo: baserow/baserow
kind: skill
stars: 5066
last_pushed: 2026-06-16T04:00:22Z
license: other
score: 9
domains: [backend-api, database-optimization]
tags: [django, sql-profiling, performance-tuning]
curated: 2026-06-16
curated_by: config-scout
---

# baserow/baserow — skill

**Why it's worth keeping:** Provides exact SQL snippets for complex tasks like normalizing query text via regex to detect patterns, and detailed instructions on navigating containerized DB environments.

**Summary:** A diagnostic workflow for investigating backend performance bottlenecks and N+1 queries using Django Silk profiling data.

**Source credibility:** Baserow is a high-star, actively maintained open-source project.

**Recency:** Highly relevant for modern agentic debugging workflows in containerized environments.

**Source:** [baserow/baserow/.agents/skills/silk-profiler/SKILL.md](https://github.com/baserow/baserow/blob/b8c8d51a46dfd845f556c52266121374a3404696/.agents/skills/silk-profiler/SKILL.md) · 5066★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: silk-profiler
description: Investigate backend performance using Django Silk profiling data. Use when investigating a slow endpoint, a potential bottleneck, N+1 queries, or understanding query patterns for a specific request.
---

# Investigate Backend Performance with Silk

Use this skill to investigate a slow endpoint or a potential bottleneck. Django Silk (enabled by default in dev via `BASEROW_ENABLE_SILK` in `dev.py`) records every HTTP request, its SQL queries, and full Python stack traces into PostgreSQL. The user may provide a Silk request URL, a request ID, or just describe which endpoint is slow.

## Prerequisites

- Silk must be enabled (default in dev: `BASEROW_ENABLE_SILK=on` in `dev.py`)
- The slow operation must have been performed recently so Silk has captured it
- The dev database must be accessible (usually via `docker exec` into the `baserow-db-1` container)

## Connecting to the Database

Read the `DATABASES` setting in `backend/src/baserow/config/settings/base.py` (and `dev.py` which imports it) to find the connection credentials. Env vars may override the defaults.

The database usually runs in a Docker container. Try `docker exec` first:

```bash
do
```

</details>
