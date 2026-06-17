---
name: lukejones3__job-market-analytics
source: https://github.com/lukejones3/job-market-analytics/blob/9a38abb0a460c1ecd20a6a5329dedc4dbea17904/CLAUDE.md
repo: lukejones3/job-market-analytics
kind: claude-md
stars: 5
last_pushed: 2026-06-11T04:28:23Z
license: other
score: 9
domains: [data-engineering, backend-api, mlops]
tags: [infrastructure-heavy, operational-context, high-precision]
curated: 2026-06-15
curated_by: config-scout
---

# lukejones3/job-market-analytics — claude-md

**Why it's worth keeping:** Contains highly actionable 'Technical gotchas' for shell operations and explicit 'Do Not' rules that ensure agentic efficiency/safety.

**Summary:** Provides deep operational context including infrastructure paths, cron schedules, and ML constraints to prevent compute waste.

**Source credibility:** High; a live production project with specific, non-generic infrastructure details.

**Recency:** Very current; addresses modern file manipulation and resource management needs.

**Source:** [lukejones3/job-market-analytics/CLAUDE.md](https://github.com/lukejones3/job-market-analytics/blob/9a38abb0a460c1ecd20a6a5329dedc4dbea17904/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — job-market-analytics

Context for Claude Code. Durable facts only. Update when structure changes.

## What this is
Python data pipeline + FastAPI + dbt powering Lander (landerjob.com), a
multi-vertical job-market analytics platform. This repo is the backend/data
layer. The Next.js frontend is a separate repo (`lander`).

## Infrastructure
- Droplet: SSH as `root@208.68.38.249`
  - ALWAYS use `root@`. `lukejones@` prompts for a password — do not use it.
- Repo on droplet: `/opt/job-market-analytics`
- DB credentials: sourced from `/opt/job-market-analytics/.env`
  (PGUSER / PGPASSWORD / PGHOST / PGDATABASE / PGPORT)
- Python venv: `/opt/job-market-analytics/.venv/bin/python` (Python 3.12.3)
- dbt binary: `/opt/job-market-analytics/.venv/bin/dbt`
- FastAPI service: `jma-api.service` (systemd, running), port 8000
- Postgres 16, database `job_analytics`, DB user `lukejones`, host `127.0.0.1`.
- dbt analytics schema: `analytics_analytics`. Marts are fully schema-qualified,
  e.g. `analytics_analytics.mart_ghost_job_index`.

## To run a psql query on the droplet
ssh root@208.68.38.249 "cd /opt/job-market-analytics && set -a && . .env && set +a && psql -c \"<SQL>\""

## Dail
```

</details>
