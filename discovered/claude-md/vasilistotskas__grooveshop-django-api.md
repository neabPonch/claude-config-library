---
name: vasilistotskas__grooveshop-django-api
source: https://github.com/vasilistotskas/grooveshop-django-api/blob/0e7efc40b21afe14cc32db11040eda9884a7b299/CLAUDE.md
repo: vasilistotskas/grooveshop-django-api
kind: claude-md
stars: 8
last_pushed: 2026-05-26T22:21:04Z
license: other
score: 10
domains: [backend-api, django, ecommerce]
tags: [django, api-design, architectural-patterns, uv-managed]
curated: 2026-06-15
curated_by: config-scout
---

# vasilistotskas/grooveshop-django-api — claude-md

**Why it's worth keeping:** It provides highly actionable guidance on custom manager optimizations and model composition, ensuring AI-generated code follows the repository's unique structural standards.

**Summary:** A comprehensive technical blueprint for a Django API that outlines command suites, architectural patterns through model mixins, and specific business logic rules.

**Source credibility:** The use of advanced patterns like optimized managers and 'uv' indicates a high-quality, professional developer codebase.

**Recency:** Extremely current, utilizing modern tooling like Python 3.14, uv, and Django 6.0.

**Source:** [vasilistotskas/grooveshop-django-api/CLAUDE.md](https://github.com/vasilistotskas/grooveshop-django-api/blob/0e7efc40b21afe14cc32db11040eda9884a7b299/CLAUDE.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

GrooveShop Django API — a headless e-commerce API built with Django 6.0 and Django REST Framework. Supports both WSGI (Gunicorn) and ASGI (Daphne/Uvicorn) with WebSocket notifications via Django Channels. Uses PostgreSQL 17, Redis, Celery (RabbitMQ broker), and Meilisearch. Python 3.14.2, managed with uv.

## Common Commands

```bash
# Install dependencies (uses uv, not pip)
uv sync --locked --all-extras --dev

# Run all tests (parallel by default via -n auto in addopts)
uv run pytest

# Run a single test file
uv run pytest tests/unit/path/to/test_file.py

# Run a single test function
uv run pytest tests/unit/path/to/test_file.py::test_function_name

# Run tests with coverage (must disable parallel with -n0)
uv run pytest --cov=. --cov-report=term --cov-report=html --cov-config=pyproject.toml -n0

# Lint and format
uv run ruff check --fix
uv run ruff format

# Run all pre-commit hooks
uv run pre-commit run --all-files

# Django management
uv run python manage.py makemigrations
uv run python manage.py migrate
uv run python manage.py runserver
uv r
```

</details>
