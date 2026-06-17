---
name: Dr4kiel__Naboo_Project
source: https://github.com/Dr4kiel/Naboo_Project/blob/4244b26b0556142107c96e95fb8412852fe4aad9/CLAUDE.md
repo: Dr4kiel/Naboo_Project
kind: claude-md
stars: 0
last_pushed: 2026-05-22T12:46:04Z
license: unknown
score: 7
domains: [web-frontend, backend-api, fullstack]
tags: [laravel, react, docker, fullstack]
curated: 2026-06-15
curated_by: config-scout
---

# Dr4kiel/Naboo_Project — claude-md

**Why it's worth keeping:** Includes explicit command mapping for both frontend and backend layers and defines clear architectural boundaries like the Service layer pattern to prevent logic bloat.

**Summary:** Provides comprehensive technical context for a full-stack React and Laravel application managed via Docker.

**Source credibility:** Low popularity; appears to be a personal/private project.

**Recency:** Very recent; aligns with modern web development workflows.

**Source:** [Dr4kiel/Naboo_Project/CLAUDE.md](https://github.com/Dr4kiel/Naboo_Project/blob/4244b26b0556142107c96e95fb8412852fe4aad9/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Naboo** (Note et Analyse du Budget Organisé et Optimisé) is a personal budget management app. Users track expenses, plan budgets, view transaction history, and generate financial reports.

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React + TypeScript, Vite, Tailwind CSS, ShadcnUI |
| Backend | PHP Laravel, Laravel Sanctum (auth) |
| Database | PostgreSQL |
| Containerization | Docker (3 services: `naboo-front`, `naboo-api`, `naboo-db`) |
| CI/CD | GitHub Actions |

## Project Structure

```
Naboo_Project/
├── front/          # React + TypeScript + Vite frontend
├── back/           # Laravel PHP backend
├── docs/           # Project documentation
│   └── GOOD_PRACTICES.md
├── docker-compose.yml
└── README.md
```

## Development Commands

### Docker (full stack)

```bash
docker compose up -d          # Start all services (front, api, db)
docker compose down           # Stop all services
docker compose logs -f api    # Follow API logs
```

### Backend (Laravel — run inside `back/`)

```bash
composer install
```

</details>
