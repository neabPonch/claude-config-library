---
name: shaptina__projem
source: https://github.com/shaptina/projem/blob/8567472674c71b04b7b169d04e5fa27102e9ee22/CLAUDE.md
repo: shaptina/projem
kind: claude-md
stars: 0
last_pushed: 2025-08-14T17:44:37Z
license: unknown
score: 9
domains: [backend-api, web-frontend, devops]
tags: [monorepo, fastapi, nextjs, workflow]
curated: 2026-06-17
curated_by: config-scout
---

# shaptina/projem — claude-md

**Why it's worth keeping:** The 'Development Workflows' provide exact step-by-step procedures for adding features, and the command documentation is exceptionally well-structured for AI execution.

**Summary:** A high-quality guide for a complex full-stack monorepo featuring FastAPI, Next.js, and Celery workers.

**Source credibility:** Low social proof (0 stars) but highly professional and structured content.

**Recency:** Highly current, featuring modern technologies like Next.js 14 and Ruff.

**Source:** [shaptina/projem/CLAUDE.md](https://github.com/shaptina/projem/blob/8567472674c71b04b7b169d04e5fa27102e9ee22/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a FreeCAD-based CNC/CAM/CAD production platform with Turkish UI/UX. Users can generate 3D models and CAM simulations through prompts or parameters, create G-code, and manage manufacturing jobs through a scalable queue system.

## Commands

### Development
```bash
# Start full development stack (API, Web, PostgreSQL, Redis, MinIO, workers)
make dev

# Start individual services
make api        # Start API only
make web        # Start web frontend only
make worker     # Start Celery workers
make beat       # Start Celery beat scheduler

# Development with hot reload
make dev-api    # API with code reload
make dev-web    # Next.js with hot reload
```

### Testing
```bash
# Run all tests
make test

# API tests
make test-api          # Run all API tests
pytest apps/api/tests  # Run specific test file/directory
pytest -k "test_name"  # Run tests matching pattern
pytest -v             # Verbose output

# Web tests
make test-web                    # Run all web tests
npm run test --prefix apps/web   # Run unit tests
npm run test:integration --pref
```

</details>
