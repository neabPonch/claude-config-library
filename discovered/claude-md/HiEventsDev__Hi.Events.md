---
name: HiEventsDev__Hi.Events
source: https://github.com/HiEventsDev/Hi.Events/blob/347ee48a6b7196a3bedba7c7e938187a21d9584e/CLAUDE.md
repo: HiEventsDev/Hi.Events
kind: claude-md
stars: 3871
last_pushed: 2026-06-04T21:45:15Z
license: other
score: 9
domains: [full-stack, backend-api, web-frontend]
tags: [laravel, react, ddd, docker, ssr]
curated: 2026-06-15
curated_by: config-scout
---

# HiEventsDev/Hi.Events — claude-md

**Why it's worth keeping:** It includes explicit shell command sequences for Docker-wrapped processes and strict 'Do/Don't' rules that prevent architectural drift. The inclusion of specific workflow steps (like regenerating domain objects after migrations) is a masterclass in preventing AI-induced technical debt.

**Summary:** A comprehensive full-stack guide that bridges the gap between high-level architecture (DDD) and low-level execution (Docker/Shell commands). It covers backend Laravel patterns, frontend React SSR constraints, and mandatory developer workflows.

**Source credibility:** High; highly starred, actively maintained open-source project.

**Recency:** Very recent; perfectly suited for modern agentic workflows that require precise shell execution instructions.

**Source:** [HiEventsDev/Hi.Events/CLAUDE.md](https://github.com/HiEventsDev/Hi.Events/blob/347ee48a6b7196a3bedba7c7e938187a21d9584e/CLAUDE.md) · 3871★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Hi.Events is an open-source event management and ticketing platform with a Laravel backend and React frontend, using Domain-Driven Design (DDD).

## Key Commands

### Backend (Laravel)

Commands must be executed in the `backend` docker container:

```bash
cd docker/development

docker compose -f docker-compose.dev.yml exec backend php artisan migrate
docker compose -f docker-compose.dev.yml exec backend php artisan generate-domain-objects
docker compose -f docker-compose.dev.yml exec backend php artisan test
docker compose -f docker-compose.dev.yml exec backend php artisan test --filter=TestName
docker compose -f docker-compose.dev.yml exec backend php artisan test --testsuite=Unit
docker compose -f docker-compose.dev.yml exec backend ./vendor/bin/pint --test
```

### Frontend (React + Vite) - SSR Only

```bash
cd frontend
yarn install
yarn dev:ssr              # Development server
yarn build                # SSR build
yarn messages:extract     # Extract translatable strings
yarn messages:compile     # Compile translations
npx tsc --noEmit
```

</details>
