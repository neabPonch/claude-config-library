---
name: divifilter__divifilter-ui
source: https://github.com/divifilter/divifilter-ui/blob/39e2136fbfcf2dd4992fb538a103e44bd534a592/CLAUDE.md
repo: divifilter/divifilter-ui
kind: claude-md
stars: 1
last_pushed: 2026-05-13T10:19:21Z
license: lgpl-3.0
score: 8
domains: [backend-api, web-app]
tags: [fastapi, htmx, mysql, python]
curated: 2026-06-16
curated_by: config-scout
---

# divifilter/divifilter-ui — claude-md

**Why it's worth keeping:** Includes critical 'gotcha' instructions regarding SQL backtick requirements for columns with spaces and clarifies the specific HTMX partial-swap pattern used.

**Summary:** A dense technical blueprint of a FastAPI/HTMX application that maps module responsibilities and execution commands.

**Source credibility:** Single-star personal project, but demonstrates high-quality documentation habits.

**Recency:** Current; aligns well with modern Python/FastAPI workflows.

**Source:** [divifilter/divifilter-ui/CLAUDE.md](https://github.com/divifilter/divifilter-ui/blob/39e2136fbfcf2dd4992fb538a103e44bd534a592/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Divifilter is a FastAPI + HTMX web app for filtering dividend stocks. It connects to a MySQL/MariaDB database containing dividend stock data and provides an interactive UI with sidebar filters (dividend metrics, financial metrics, exclusions). Results display as a pandas DataFrame table rendered as HTML, updated via HTMX partial swaps without full page reloads.

## Commands

```bash
# Run the app locally (requires DB connection via env vars or config files)
uvicorn dividend_stocks_filterer.app:app --host 0.0.0.0 --port 8080 --reload

# Run all tests
coverage run -m unittest

# Lint (matches CI config)
flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics

# Docker
docker build -t divifilter-ui .
docker run -p 80:80 divifilter-ui

# Health check
curl http://localhost:8080/health
```

## Architecture

Five modules in `dividend_stocks_filterer/`:

- **app.py** — FastAPI entry point. Computes all slider range values once at startup from DB min/max queries
```

</details>
