---
name: l3ocho__app-personal-portfolio-dataflow
source: https://github.com/l3ocho/app-personal-portfolio-dataflow/blob/cbe1fd59314f9b8668177c1efe50b33071e562d5/CLAUDE.md
repo: l3ocho/app-personal-portfolio-dataflow
kind: claude-md
stars: 0
last_pushed: 2026-03-29T21:52:20Z
license: mit
score: 9
domains: [data-engineering, etl, backend]
tags: [dbt, impact-analysis, data-contracts, pipeline]
curated: 2026-06-17
curated_by: config-scout
---

# l3ocho/app-personal-portfolio-dataflow — claude-md

**Why it's worth keeping:** The 'Impact Analysis' table is a masterclass in prompting; it provides exact commands (dbt lineage/grep) to force the agent to verify downstream impacts before changing schemas.

**Summary:** A highly sophisticated instruction set for a data engineering pipeline that emphasizes cross-repository dependency management and strict data contracts.

**Source credibility:** Individual developer portfolio repo with high technical density and clear documentation standards.

**Recency:** Very recent (3 months ago), perfectly aligned with modern AI coding workflows.

**Source:** [l3ocho/app-personal-portfolio-dataflow/CLAUDE.md](https://github.com/l3ocho/app-personal-portfolio-dataflow/blob/cbe1fd59314f9b8668177c1efe50b33071e562d5/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

> See `~/.claude/CLAUDE.md` for global behavior rules that apply to this and all projects.

---

## Project Overview

**Repository**: personal-portfolio-dataflow
**Purpose**: Data engineering pipeline (ETL/ELT) for analytics projects
**Scope**: Data acquisition → Database persistence (NO FRONTEND)

This is a **data-only** repository. All visualization and frontend code lives in the separate `personal-portfolio` webapp repository.

---

## Project Status

**Last Completed Sprint**: 10 (Dataflow Separation & Production Deployment)
**Current State**: Production-ready data pipeline
**Branch**: `development` (feature branches merge here)

---

## Quick Reference

### Run Commands

```bash
# Setup & Database
make setup          # Install deps, create .env, init pre-commit
make local-dev      # Full dev stack: docker-up + db-init + pgweb (http://localhost:8081)
make docker-up      # Start PostgreSQL + PostGIS only (no pgweb)
make docker-down    # Stop containers
make db-init        # Initialize database schema
make db-reset       # Drop and recreate database (DESTRUCTIVE)

# Data Loading
make load-data      # Load all project data (currently: Toronto)
make load-toronto   # Lo
```

</details>
