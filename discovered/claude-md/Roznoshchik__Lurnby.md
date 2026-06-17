---
name: Roznoshchik__Lurnby
source: https://github.com/Roznoshchik/Lurnby/blob/5479480fa6f681de5524a206f4ae32932f82b81f/CLAUDE.md
repo: Roznoshchik/Lurnby
kind: claude-md
stars: 703
last_pushed: 2026-05-01T14:46:54Z
license: bsd-3-clause
score: 9
domains: [web-fullstack, python-flask, javascript-preact]
tags: [architecture-mapping, migration-context, dev-ops]
curated: 2026-06-14
curated_by: config-scout
---

# Roznoshchik/Lurnby — claude-md

**Why it's worth keeping:** The explicit mapping of blueprint structures, asset resolution logic (dev vs prod), and detailed data model relationships prevents AI hallucination during refactoring.

**Summary:** Provides high-density architectural context for a complex full-stack migration from Jinja2 to Preact.

**Source credibility:** High; significant star count and recent activity indicate a real-world production environment.

**Recency:** Very current; updated within the last month.

**Source:** [Roznoshchik/Lurnby/CLAUDE.md](https://github.com/Roznoshchik/Lurnby/blob/5479480fa6f681de5524a206f4ae32932f82b81f/CLAUDE.md) · 703★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project Overview

Lurnby is a personal knowledge practice tool built with Flask that helps users read and remember more through active recall and spaced repetition. It supports web articles and epubs with highlighting, categorization, and review features.

**Tech Stack:**
- Backend: Flask, SQLAlchemy, PostgreSQL, Redis
- Frontend: Preact + Vite (active migration from Jinja2 templates), JavaScript, CSS
- Background Tasks: RQ (Redis Queue)
- External Services: AWS S3 (epub images), Google OAuth, SendGrid (email)
- Deployment: Heroku (via git push using Dockerfile)
- Testing: pytest (backend), Vitest (frontend)

## Development Setup

### Initial Setup
```bash
# Create and activate virtual environment
python3 -m venv venv
. venv/bin/activate

# Install Python dependencies
pip install -r requirements.txt

# Install Node.js dependencies for Preact frontend
cd client && npm install && cd ..

# Setup database
flask db upgrade

# Create .env file from .env.example
cp .env.example .env
# Edit .env with required credentials
```

### Running the Application

```bash
just serve        # Dev mode: Redis → RQ → Vite → Flask
just serve-prod   # Prod mode: builds assets first
```

### Testing
```
```

</details>
