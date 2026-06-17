---
name: ohcnetwork__care
source: https://github.com/ohcnetwork/care/blob/bb3f442e0a8e3901487965676dc17e04e012a0f8/CLAUDE.md
repo: ohcnetwork/care
kind: claude-md
stars: 376
last_pushed: 2026-06-14T16:38:38Z
license: mit
score: 9
domains: [backend-api, python-django]
tags: [django, ruff, docker, workflow]
curated: 2026-06-14
curated_by: config-scout
---

# ohcnetwork/care — claude-md

**Why it's worth keeping:** The 'Autonomous AI Workflow' section is gold; it provides explicit sequential instructions for an agent to follow. It also includes exact shell commands/environment variables, eliminating guesswork during setup.

**Summary:** A comprehensive guide that covers environment setup (Docker and venv), detailed project architecture, and specific tool requirements.

**Source credibility:** High: Active repository (last pushed 0 months ago) with significant social proof (376 stars).

**Recency:** Extremely current; utilizes Python 3.13 and modern tooling like Ruff.

**Source:** [ohcnetwork/care/CLAUDE.md](https://github.com/ohcnetwork/care/blob/bb3f442e0a8e3901487965676dc17e04e012a0f8/CLAUDE.md) · 376★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What is CARE?

CARE is a Digital Public Good building an open source EMR + Hospital Management system. This is the Django backend (Django 6.0 + Python 3.13 + PostgreSQL + Redis).

## Local Development Environment

### Running Locally (without Docker)

The local setup uses a Python 3.13 venv with PostgreSQL 16 and Redis running natively.

**Start services:**
```bash
# Ensure PostgreSQL 16 and Redis are running on your system
# Start Django backend on port 9000
DJANGO_SETTINGS_MODULE=config.settings.local DJANGO_READ_DOT_ENV_FILE=true .venv/bin/python manage.py runserver 0.0.0.0:9000
```

**Database:**
- PostgreSQL on localhost:5432, database `care`, user `postgres`, password `postgres`
- Config in `.env` (gitignored)

### Running with Docker

```bash
cp .env.example .env
make up               # Start all services (db, redis, minio, backend, celery)
make load-fixtures    # Load test data
make logs             # View logs
make down             # Stop services
```

## Build/Test Commands

### With Docker (Makefile)
- `make up` — Start all services
- `make build` — Bui
```

</details>
