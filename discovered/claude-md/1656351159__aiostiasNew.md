---
name: 1656351159__aiostiasNew
source: https://github.com/1656351159/aiostiasNew/blob/e3b0213eb9aa7abf48476067570c57ffe7e36867/CLAUDE.md
repo: 1656351159/aiostiasNew
kind: claude-md
stars: 0
last_pushed: 2026-05-08T11:56:43Z
license: unknown
score: 9
domains: [backend-api, web-frontend, automation, embedded-systems]
tags: [multi-service, architecture-mapping, technical-debt-warning]
curated: 2026-06-16
curated_by: config-scout
---

# 1656351159/aiostiasNew — claude-md

**Why it's worth keeping:** The 'Important Implementation Details' section is excellent; it preemptively warns the AI about hardcoded Windows paths, SQL syntax quirks, and proxy configurations that would otherwise cause bugs.

**Summary:** A highly detailed multi-service documentation that maps ports, service interactions, and deployment commands across a complex stack.

**Source credibility:** Low social proof (0 stars) but high-quality technical documentation density.

**Recency:** Current, utilizing modern stacks like React 19 and FastAPI.

**Source:** [1656351159/aiostiasNew/CLAUDE.md](https://github.com/1656351159/aiostiasNew/blob/e3b0213eb9aa7abf48476067570c57ffe7e36867/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

AI-OSTIAS (AI-driven Open Source Technology Intelligence Analysis Software) is an aerospace/defense intelligence collection and analysis platform. Three active services + one embedded firmware:

- **ostias-frontend/** — React 19 SPA, port 15173
- **ostias-backend/** — Express + MySQL, port 15000 (article CRUD, REST API, crawl trigger)
- **ostias-openclaw/** — FastAPI + Playwright, port 18790 (browser automation + LLM proxy)
- **hi3861_env_monitor/** — Hi3861 embedded C firmware (decoupled from main stack)

The core differentiator is "programmable browser intelligence" — Playwright-driven action sequences with anti-detection, full trace logging, and AI-driven extraction replacing hardcoded parsers.

For detailed architecture, roadmap, and progress, see `README.md`.

## Common Development Commands

### Frontend (`ostias-frontend/`)
```bash
npm install
npm run dev      # http://127.0.0.1:15173
npm run build
npm run lint
```

### Backend (`ostias-backend/`)
```bash
npm install
npm start        # port 15000

# With Docker:
docker-compose up -d   # MyS
```

</details>
