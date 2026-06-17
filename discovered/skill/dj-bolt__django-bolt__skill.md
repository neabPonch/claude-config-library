---
name: dj-bolt__django-bolt__skill
source: https://github.com/dj-bolt/django-bolt/blob/e1390e95b4c5367030a2992a8e47f651cc3fd2e8/.agents/django-bolt/SKILL.md
repo: dj-bolt/django-bolt
kind: skill
stars: 1531
last_pushed: 2026-06-14T21:07:27Z
license: unknown
score: 9
domains: [backend-api, python, high-performance]
tags: [django, rust, msgspec, async]
curated: 2026-06-16
curated_by: config-scout
---

# dj-bolt/django-bolt — skill

**Why it's worth keeping:** Features excellent negative constraints to prevent hallucinating standard Django patterns and uses highly detailed code examples for complex typing with `msgspec` and `Annotated` markers.

**Summary:** A specialized skill file for the high-performance Django-Bolt framework that provides specific async/type-safety patterns.

**Source credibility:** High; the source repo is well-starred, actively maintained, and provides a specific high-performance niche.

**Recency:** Current; utilizes modern Python 3.10+ syntax like union types and `Annotated` structures.

**Source:** [dj-bolt/django-bolt/.agents/django-bolt/SKILL.md](https://github.com/dj-bolt/django-bolt/blob/e1390e95b4c5367030a2992a8e47f651cc3fd2e8/.agents/django-bolt/SKILL.md) · 1531★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: django-bolt
description: Build high-performance APIs with Django-Bolt, including BoltAPI routes, typed request validation, msgspec serialization, auth guards, middleware, OpenAPI docs, pagination, streaming, SSE, WebSockets, and testing. Use when the user asks to create a new bolt endpoint, set up a Django-Bolt project, add JWT or API key auth, configure runbolt, wire guards or middleware, add pagination or streaming, generate OpenAPI docs, write TestClient tests, or migrate from FastAPI, Django REST Framework, or Django Ninja to django-bolt. Do NOT use for general Django views, Django admin customization, or standard Django REST Framework work.
compatibility: Skills-compatible coding agents working on Django projects that use django-bolt.
metadata:
  author: Farhan Ali Raza
  category: web-framework
  version: 0.7.0
  tags: [django, django-bolt, api, rust, high-performance, openapi, testing]
---

# Django-Bolt

## Critical rules

- Always use async handlers unless the user explicitly needs sync
- Use async database access in async handlers (e.g., Django async ORM: `aget`, `acreate`, `afilter`)
- Use `msgspec.Struct` for simple typed payloads; use `Serializer` for richer
```

</details>
