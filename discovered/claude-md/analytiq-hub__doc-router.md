---
name: analytiq-hub__doc-router
source: https://github.com/analytiq-hub/doc-router/blob/7cc0d312cde1a441cf026d83c2987f8e0caf65a7/CLAUDE.md
repo: analytiq-hub/doc-router
kind: claude-md
stars: 25
last_pushed: 2026-06-16T16:49:21Z
license: apache-2.0
score: 9
domains: [fullstack, python, typescript]
tags: [monorepo, architecture-guide, dev-workflow]
curated: 2026-06-16
curated_by: config-scout
---

# analytiq-hub/doc-router — claude-md

**Why it's worth keeping:** Includes explicit 'do not' rules to prevent subtle bugs and a sophisticated cross-repo reference guide that provides external context through a sibling repository.

**Summary:** Provides comprehensive technical context including build commands, architectural patterns, service endpoints, and specific guardrails.

**Source credibility:** High; the detail suggests an active, professional multi-service project.

**Recency:** Current; references modern stacks like NextJS 14 App Router and specific Python toolchains.

**Source:** [analytiq-hub/doc-router/CLAUDE.md](https://github.com/analytiq-hub/doc-router/blob/7cc0d312cde1a441cf026d83c2987f8e0caf65a7/CLAUDE.md) · 25★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Setup and Installation
- The Python virtual environment is **`.venv` at the repository root**. Activate it from the repo top: `. .venv/bin/activate` (not from `packages/python` alone).
- `make setup` - Set up Python virtual environment and install all dependencies
- `make dev` - Start all development services (equivalent to `./start-all.sh`)
- `make tests` - Run Python tests in packages/python/tests/
- `make clean` - Remove virtual environment

### Frontend (NextJS)
Navigate to `packages/typescript/frontend/` directory:
- `npm run dev` - Start development server on port 3000
- `npm run build` - Build production bundle
- `npm run start` - Start production server
- `npm run lint` - Run ESLint

### Backend (FastAPI)
From `packages/` directory with activated virtual environment:
- `uvicorn app.main:app --reload --host 0.0.0.0 --port 8000` - Start development server
- `python worker/worker.py` - Start background worker process

### Testing
- `. .venv/bin/activate; pytest -n auto packages/python/tests/` - Run all Python tests with parallel exec
```

</details>
