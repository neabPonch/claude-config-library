---
name: indrz__indrz-be
source: https://github.com/indrz/indrz-be/blob/3769233fe2013ecd58d98032b44c96fc84fe7da1/CLAUDE.md
repo: indrz/indrz-be
kind: claude-md
stars: 118
last_pushed: 2026-05-03T20:37:36Z
license: other
score: 9
domains: [full-stack, web-development, django, vue]
tags: [architecture-driven, workflow-optimized, context-hierarchy]
curated: 2026-06-14
curated_by: config-scout
---

# indrz/indrz-be — claude-md

**Why it's worth keeping:** The 'Read This First' hierarchy instructs the agent on how to build mental models before coding, while 'Golden Rules' enforce strict engineering constraints like domain scoping.

**Summary:** Provides structured context via a prioritized reading order and detailed architectural maps for a complex full-stack environment.

**Source credibility:** High; 118 stars indicates a legitimate project with active maintenance.

**Recency:** Current; explicitly references Claude Code and modern tech stacks.

**Source:** [indrz/indrz-be/CLAUDE.md](https://github.com/indrz/indrz-be/blob/3769233fe2013ecd58d98032b44c96fc84fe7da1/CLAUDE.md) · 118★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 1. Purpose

Indrz is an indoor mapping, fm management platform.

## 2. Read This First

Before making changes, read in this order:

1. **For Product Understanding**: Start with product specs (`docs/specification/*.md`)
2. **For Implementation**: Reference technical specs (`spec-*-techstack.md`)
3. **For Feature Dependencies**: Check "Related Specifications" sections in each doc
4. **For Writing New Specs**: Use [TEMPLATE.md](./TEMPLATE.md)

## 3. Repo Map

- `backend/` — API, Django + DRF + PostGIS, PgRouting, Geoserver
- `frontend/` — Nuxt 4 + Vue 3 + Vuetify 3 + OpenLayers
- `devops/` — dockerfiles to build images
- `docs/specification` — application specifications for AI context
- `docs/user/` — user facing documentation in both english and german


## 4. Development Commands

### Docker-first local development (recommended)

```bash
# Start all services (PostGIS, Django API, GeoServer, Nuxt dev server, Nginx)
make up

# Start only PostGIS database and Django API
make up-api

# stop only PostGIS database and Django API
make down-api

# Stop all services
make do
```

</details>
