---
name: LiorCohen__sdd__claude-tmpl
source: https://github.com/LiorCohen/sdd/blob/a8a1cadb48f764aa6ab8f9a4ea6639a9de6863b1/plugin/fullstack-typescript/templates/project/CLAUDE.md.tmpl
repo: LiorCohen/sdd
kind: claude-md
stars: 32
last_pushed: 2026-02-24T08:17:23Z
license: unknown
score: 9
domains: [backend-api, architecture, fullstack, agentic-workflows]
tags: [spec-driven, architectural-patterns, coding-standards, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# LiorCohen/sdd — claude-md

**Why it's worth keeping:** The mandatory standards lookup table prevents context drift by forcing the agent to load specific rules per layer, and the CMDO architecture provides a rigid mental model for code generation.

**Summary:** Implements a highly structured Spec-Driven Development (SDD) framework that mandates task-specific 'standards skills' to ensure architectural consistency.

**Source credibility:** 32 stars indicates a specialized tool/plugin that has gained traction within its niche of spec-driven workflows.

**Recency:** Extremely current; references React 19 and modern agentic workflow patterns suitable for Claude Code.

**Source:** [LiorCohen/sdd/plugin/fullstack-typescript/templates/project/CLAUDE.md.tmpl](https://github.com/LiorCohen/sdd/blob/a8a1cadb48f764aa6ab8f9a4ea6639a9de6863b1/plugin/fullstack-typescript/templates/project/CLAUDE.md.tmpl) · 32★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project: {{PROJECT_NAME}}

## Tech Stack

- **API Contract:** OpenAPI 3.x (path depends on contract component name in `sdd/sdd-settings.yaml`)
- **Backend:** Node.js 20, TypeScript 5, Express (CMDO architecture)
- **Frontend:** React 19, TypeScript 5.9, Vite (MVVM architecture)
- **Database:** PostgreSQL 15
- **Testing:** Vitest (unit), Testkube (integration/E2E)
- **Deployment:** Kubernetes, Helm

## Components

| Component | Path | Purpose |
|-----------|------|---------|
| Config | `components/config/` | Environment configuration (mandatory singleton) |
| Contract | `components/contracts/{name}/` | OpenAPI spec, type generation |
| Server | `components/servers/{name}/` | Backend (CMDO architecture) |
| Webapp | `components/webapps/{name}/` | React frontend (MVVM) |
| Database | `components/databases/{name}/` | PostgreSQL migrations and seeds |
| Helm | `components/helm_charts/{name}/` | Kubernetes deployment |
| Testing | `components/testing/{name}/` | Testkube test definitions |

Component directories follow the pattern `components/{type-plural}/{name}/` (e.g., `components/contracts/public-api/`, `components/servers/main/`).

## Backend Architecture (CMDO)

**C**ontroller **M
```

</details>
