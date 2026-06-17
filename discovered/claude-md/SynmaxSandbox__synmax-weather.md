---
name: SynmaxSandbox__synmax-weather
source: https://github.com/SynmaxSandbox/synmax-weather/blob/2c2594e5179ee1331fdc82bbe9e39a01ee98816b/claude.md
repo: SynmaxSandbox/synmax-weather
kind: claude-md
stars: 0
last_pushed: 2026-02-12T15:20:06Z
license: unknown
score: 8
domains: [backend-api, data-science, geospatial]
tags: [fastapi, nextjs, geospatial, architectural-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# SynmaxSandbox/synmax-weather — claude-md

**Why it's worth keeping:** It includes high-value 'domain wisdom'—specifically advising on vectorized operations to prevent inefficient data transfers—and provides clear procedural patterns for common tasks like adding endpoints or regions.

**Summary:** Provides a comprehensive map of architecture, operational commands, and domain-specific technical constraints for a weather forecasting platform.

**Source credibility:** The repository has low social proof (0 stars), but the technical specificity and complex stack suggest a genuine, functional project.

**Recency:** 

**Source:** [SynmaxSandbox/synmax-weather/claude.md](https://github.com/SynmaxSandbox/synmax-weather/blob/2c2594e5179ee1331fdc82bbe9e39a01ee98816b/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SynMax Weather

Weather forecasting benchmark platform - a monolith backend with Next.js dashboard.

For local development, use the synmax-weather environment. If it is not set up, set it up first using the requirements.txt file.

For new features, first checkout a new branch on git and do development there

Be efficient about geospatial data queries, code generation and handling. For example, while querying data for polygons in a raster, use vectorized operations, and don't fetch the entire dataset from remote to local first. Try to minimize large data transfers.

## Architecture

```
synmax-weather/
├── backend/              # Single FastAPI service
│   ├── app/
│   │   ├── api/v1/       # All endpoints
│   │   ├── core/         # Config, DB, cache
│   │   ├── services/     # Business logic
│   │   ├── models/       # SQLAlchemy ORM
│   │   └── schemas/      # Pydantic
│   ├── tests/
│   └── notebooks/
├── dashboard/            # Next.js frontend
└── docker-compose.yml
```

## Running Locally

```bash
# Infrastructure
docker-compose -f docker-compose.yml -f docker-compose.dev.yml up -d

# Backend (port 8000)
cd backend
conda activate synmax-weather
uvicorn app.main:app --reload
```

</details>
