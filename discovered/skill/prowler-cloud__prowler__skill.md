---
name: prowler-cloud__prowler__skill
source: https://github.com/prowler-cloud/prowler/blob/dc3433aaf0d18c2d548579a80902f8ee2f185ad8/skills/prowler-api/SKILL.md
repo: prowler-cloud/prowler
kind: skill
stars: 13997
last_pushed: 2026-06-14T20:05:26Z
license: apache-2.0
score: 9
domains: [backend-api, security, database-architecture]
tags: [django, rls, rbac, multitenancy]
curated: 2026-06-15
curated_by: config-scout
---

# prowler-cloud/prowler — skill

**Why it's worth keeping:** It provides essential 'Critical Rules' to prevent security bypasses and utilizes decision trees/checklists that translate complex tribal knowledge into actionable agent instructions.

**Summary:** This config outlines critical architectural patterns for the Prowler API, specifically focusing on tenant-scoped Row-Level Security (RLS) and multi-database routing.

**Source credibility:** High; Prowler is a highly-starred, widely used open-source cloud security platform.

**Recency:** Current; uses modern patterns for Django, Celery, and PostgreSQL RLS implementation.

**Source:** [prowler-cloud/prowler/skills/prowler-api/SKILL.md](https://github.com/prowler-cloud/prowler/blob/dc3433aaf0d18c2d548579a80902f8ee2f185ad8/skills/prowler-api/SKILL.md) · 13997★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: prowler-api
description: >
  Prowler API patterns: RLS, RBAC, providers, Celery tasks.
  Trigger: When working in api/ on models/serializers/viewsets/filters/tasks involving tenant isolation (RLS), RBAC, or provider lifecycle.
license: Apache-2.0
metadata:
  author: prowler-cloud
  version: "1.2.0"
  scope: [root, api]
  auto_invoke: "Creating/modifying models, views, serializers"
allowed-tools: Read, Edit, Write, Glob, Grep, Bash, WebFetch, WebSearch, Task
---

## When to Use

Use this skill for **Prowler-specific** patterns:
- Row-Level Security (RLS) / tenant isolation
- RBAC permissions and role checks
- Provider lifecycle and validation
- Celery tasks with tenant context
- Multi-database architecture (4-database setup)

For **generic DRF patterns** (ViewSets, Serializers, Filters, JSON:API), use `django-drf` skill.

---

## Critical Rules

- ALWAYS use `rls_transaction(tenant_id)` when querying outside ViewSet context
- ALWAYS use `get_role()` before checking permissions (returns FIRST role only)
- ALWAYS use `@set_tenant` then `@handle_provider_deletion` decorator order
- ALWAYS use explicit through models for M2M relationships (required for RLS)
- NEVER access `Pro
```

</details>
