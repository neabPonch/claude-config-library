---
name: SRamoras__e_commerce_platform
source: https://github.com/SRamoras/e_commerce_platform/blob/fc86a7b0f6853e53b9d4a64f60cf1557d981dfb2/Claude.md
repo: SRamoras/e_commerce_platform
kind: claude-md
stars: 0
last_pushed: 2026-04-05T05:09:34Z
license: unknown
score: 9
domains: [backend, web-development]
tags: [django, schema-driven, architectural-blueprint]
curated: 2026-06-16
curated_by: config-scout
---

# SRamoras/e_commerce_platform — claude-md

**Why it's worth keeping:** Uses explicit schema definitions (fields, types, and logic rules) to prevent AI hallucination of business requirements. The 'Rules' sections within models provide excellent examples of how to instruct an agent on data integrity and constraints.

**Summary:** A highly detailed architectural blueprint for a Django e-commerce system, defining specific project structures, URL patterns, and granular model schemas.

**Source credibility:** Low-signal source (0 stars), likely a personal demo repo, but the content itself is high-quality documentation.

**Recency:** Very current; uses modern versions like Django 6 and Python 3.12.

**Source:** [SRamoras/e_commerce_platform/Claude.md](https://github.com/SRamoras/e_commerce_platform/blob/fc86a7b0f6853e53b9d4a64f60cf1557d981dfb2/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — djangodemostore

This file is the authoritative instruction set for Claude Code when working on this project.
Read it in full before taking any action. Follow every constraint exactly as written.
When in doubt, ask rather than assume.

---

## 1. Project Overview

**djangodemostore** is a demonstration e-commerce platform built with Django 6.
It is not a production system. Payment processing is mocked. Download delivery for digital
products is not implemented. The goal is a clean, well-structured codebase that demonstrates
correct Django patterns at every layer.

---

## 2. Technology Stack

| Layer | Technology | Notes |
|---|---|---|
| Web framework | Django 6 | Use async views only where explicitly instructed |
| Language | Python 3.12+ | Type hints encouraged but not mandatory |
| Database | PostgreSQL 16 | Via psycopg3 (`psycopg[binary]`) |
| Cache / Sessions | Redis 7 | django-redis backend |
| Partial API | Django REST Framework | Cart and Search endpoints only |
| Task queue | Celery + Redis broker | Scaffolded only -- no actual tasks |
| Frontend | Django Templates + HTMX | No React, no Vue, no iframes |
| Containerisation | Docker Compose | Three services on
```

</details>
