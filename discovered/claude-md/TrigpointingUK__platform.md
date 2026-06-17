---
name: TrigpointingUK__platform
source: https://github.com/TrigpointingUK/platform/blob/7f9780a489e08964aebc707c974c8ba055149af3/CLAUDE.md
repo: TrigpointingUK/platform
kind: claude-md
stars: 1
last_pushed: 2026-06-12T12:34:54Z
license: agpl-3.0
score: 10
domains: [backend-api, web-frontend, devops]
tags: [monorepo, fullstack, deployment-rules, technical-debt-prevention]
curated: 2026-06-15
curated_by: config-scout
---

# TrigpointingUK/platform — claude-md

**Why it's worth keeping:** Includes high-value 'gotcha' prevention (SQLAlchemy join patterns/Tailwind v4 syntax) and utilizes a sophisticated 'skill' pattern for secure database access via tunnels.

**Summary:** Provides a comprehensive structural map of a monorepo with specific command patterns for backend, frontend, and infrastructure. It includes critical business logic nuances and environment synchronization rules.

**Source credibility:** High; the technical specificity regarding historical bugs suggests an expert maintainer.

**Recency:** Extremely current, referencing React 19 and Tailwind v4.

**Source:** [TrigpointingUK/platform/CLAUDE.md](https://github.com/TrigpointingUK/platform/blob/7f9780a489e08964aebc707c974c8ba055149af3/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository overview

Monorepo for **Trigpointing.uk**, a long-running trigpoint/surveying community site. Multiple deployable units share infrastructure:

- [api/](api/) — FastAPI (Python 3.11+) REST API. Entry point [api/main.py](api/main.py); endpoints under [api/api/v1/](api/api/v1/); business logic in [api/services/](api/services/); SQLAlchemy models in [api/models/](api/models/); CRUD in [api/crud/](api/crud/); Pydantic schemas in [api/schemas/](api/schemas/); tests in [api/tests/](api/tests/).
- [web/](web/) — React 19 + TypeScript SPA built with Vite 8, TanStack Query, React Router 7, Auth0 PKCE, Tailwind v4. Source under [web/src/](web/src/).
- [forum/](forum/) — phpBB 3.3 with Auth0 SSO (production only, no staging).
- [wiki/](wiki/) — MediaWiki with Auth0 SSO (production only, no staging).
- [terraform/](terraform/) — AWS IaC, split into [common/](terraform/common/), [staging/](terraform/staging/), [production/](terraform/production/), and reusable [modules/](terraform/modules/). ECS Fargate behind ALB, RDS PostgreSQL, Valkey (Redis-compatible) ElastiCac
```

</details>
