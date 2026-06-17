---
name: c0x12c__ai-toolkit__skill
source: https://github.com/c0x12c/ai-toolkit/blob/965f256bda59d78df779d548f892fc31dd0cb2cd/toolkit/skills/python-api-endpoint-creator/SKILL.md
repo: c0x12c/ai-toolkit
kind: skill
stars: 79
last_pushed: 2026-05-11T06:56:56Z
license: unknown
score: 8
domains: [backend-api, python]
tags: [fastapi, layered-architecture, rest-api, sql-alchemy]
curated: 2026-06-15
curated_by: config-scout
---

# c0x12c/ai-toolkit — skill

**Why it's worth keeping:** The 'Gotchas' and 'Hard Rules' sections provide high-value defensive programming instructions that prevent common architectural mistakes like leaking internal models or mishandling database commits.

**Summary:** Enforces a strict layered architecture (Router-Service-Repository) for FastAPI applications to ensure separation of concerns.

**Source credibility:** Low star count, but highly specialized content suggests a developer with specific domain expertise.

**Recency:** 

**Source:** [c0x12c/ai-toolkit/toolkit/skills/python-api-endpoint-creator/SKILL.md](https://github.com/c0x12c/ai-toolkit/blob/965f256bda59d78df779d548f892fc31dd0cb2cd/toolkit/skills/python-api-endpoint-creator/SKILL.md) · 79★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: python-api-endpoint-creator
description: "Creates FastAPI endpoints with layered architecture (Router → Service → Repository). Use when creating new API endpoints, CRUD operations, or scaffolding a new domain module in a FastAPI project."
allowed_tools:
  - Read
  - Write
  - Edit
  - Glob
  - Grep
---

# Python API Endpoint Creator

Creates complete FastAPI endpoints following strict layered architecture patterns.

## When to Use

- Creating a new REST API endpoint from scratch
- Adding CRUD operations for a new domain entity
- Setting up the full stack: Router → Service → Repository → Tests
- Scaffolding a new domain module

## Process

1. **Pydantic Schemas** — Create/Update/Response in `schemas.py`
2. **SQLAlchemy Model** — with SoftDeleteMixin in `models.py`
3. **Repository** — async CRUD with soft delete in `repository.py`
4. **Service** — business logic, HTTPException for errors in `service.py`
5. **Dependencies** — `get_db`, `get_service` in `dependencies.py`
6. **Router** — thin endpoints, Depends() for everything in `router.py`
7. **Tests** — httpx AsyncClient tests in `tests/`

> See code-patterns.md for complete templates for each file.

## Architecture

```
R
```

</details>
