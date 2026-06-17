---
name: michaelklos__feverish
source: https://github.com/michaelklos/feverish/blob/3dfc686d3247c1cd0ae9f46555543df87c36b81d/claude.md
repo: michaelklos/feverish
kind: claude-md
stars: 1
last_pushed: 2026-05-06T12:13:56Z
license: unknown
score: 9
domains: [backend-api, django, devops]
tags: [django, architecture, azure, deployment-guide]
curated: 2026-06-15
curated_by: config-scout
---

# michaelklos/feverish — claude-md

**Why it's worth keeping:** Excellent use of a 'Design Decisions' section to prevent LLM-induced regressions; includes highly actionable CLI command blocks for local, Docker, and Cloud environments.

**Summary:** Provides comprehensive architectural, operational, and technical specification for a Django-based API project deployed on Azure.

**Source credibility:** Low star count, but the file structure indicates a high-quality personal engineering project.

**Recency:** 

**Source:** [michaelklos/feverish/claude.md](https://github.com/michaelklos/feverish/blob/3dfc686d3247c1cd0ae9f46555543df87c36b81d/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Feverish - Claude Code Context

## Project Overview

Feverish is a self-hosted RSS reader backend implementing the Fever API v3 specification. It's a personal tool for the owner, deployed on Azure Container Apps, allowing use of Fever-compatible RSS clients like Reeder.

**Production URL:** `https://news.klos.wtf`

## Tech Stack

- **Framework:** Django 6.0 / Python 3.12+
- **Database:** PostgreSQL via Neon Serverless (production), SQLite (local dev)
- **Hosting:** Azure Container Apps (scale-to-zero)
- **Package Manager:** uv
- **CI/CD:** GitHub Actions

## Architecture

```
┌─────────────────┐     ┌─────────────────┐
│  Reeder / RSS   │────▶│  feverish-web   │
│     Client      │     │  (Django API)   │
└─────────────────┘     └────────┬────────┘
                                 │
                                 ▼
                        ┌─────────────────┐
                        │  Neon Postgres  │
                        └────────┬────────┘
                                 │
┌─────────────────┐              │
│ feverish-worker │──────────────┘
│  (Hourly Cron)  │
└─────────────────┘
```

- **feverish-web:** Django app serving the Fever API (scale-to-zero, 10-15s cold start)
```

</details>
