---
name: Dorian-APHM__OPAL
source: https://github.com/Dorian-APHM/OPAL/blob/be94bde2ad4853ec0c7a8e20b116ebec852da207/CLAUDE.md
repo: Dorian-APHM/OPAL
kind: claude-md
stars: 1
last_pushed: 2026-06-13T19:43:17Z
license: apache-2.0
score: 9
domains: [backend-api, fullstack-web, data-engineering]
tags: [architecture-map, environment-config, module-inventory]
curated: 2026-06-15
curated_by: config-scout
---

# Dorian-APHM/OPAL — claude-md

**Why it's worth keeping:** Includes critical environmental 'Network' warnings to prevent proxy errors; uses highly detailed module descriptions that act as a mental map for navigating complex business logic.

**Summary:** Provides comprehensive project context including environment-specific network instructions and a granular module map of the backend API surface.

**Source credibility:** Low star count, but the technical depth suggests a sophisticated real-world medical data platform.

**Recency:** 

**Source:** [Dorian-APHM/OPAL/CLAUDE.md](https://github.com/Dorian-APHM/OPAL/blob/be94bde2ad4853ec0c7a8e20b116ebec852da207/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

OPAL (OMOP Platform for Analytics & Lineage) is a full-stack web application for analyzing OMOP CDM (Common Data Model) databases. It provides data quality analysis, cohort building, vocabulary mapping, and concept exploration. The application connects read-only to external OMOP CDM PostgreSQL databases while storing all application state in its own internal PostgreSQL database.

## Commands

> **Network**: this environment has direct internet access — **no HTTP proxy is required** for any install or build (`npm install`, `pip install`, `docker compose build`, etc.). Do not pass `HTTP_PROXY`/`HTTPS_PROXY` build-args or `--build-arg` proxy flags.

### Full Stack (Docker Compose)
```bash
export SECRET_KEY=$(openssl rand -hex 32)
export POSTGRES_PASSWORD=yourpassword
docker compose up -d          # Start all services
docker compose down            # Stop all services
```

### Backend Development
```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload --port 8000
```

### Frontend Development
```bash
cd frontend
npm install
npm r
```

</details>
