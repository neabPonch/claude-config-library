---
name: eric-maynard__riftfound
source: https://github.com/eric-maynard/riftfound/blob/89622dfd9de088b5898673d8b0dc77573ecaa0ed/CLAUDE.md
repo: eric-maynard/riftfound
kind: claude-md
stars: 5
last_pushed: 2026-05-10T06:21:51Z
license: apache-2.0
score: 9
domains: [web-frontend, backend-api, infrastructure-as-code, devops]
tags: [serverless, aws, architecture, cli-workflows]
curated: 2026-06-17
curated_by: config-scout
---

# eric-maynard/riftfound — claude-md

**Why it's worth keeping:** Contains exact command-line patterns for dev/deploy modes and specific AWS CLI commands for log inspection that an agent can execute.

**Summary:** Provides a high-density technical overview of architecture, environment setup, and operational workflows.

**Source credibility:** Legitimate project with recent maintenance (1 month ago) and 5 stars on GitHub.

**Recency:** Current; reflects modern serverless/IaC patterns including Terraform and AWS Lambda.

**Source:** [eric-maynard/riftfound/CLAUDE.md](https://github.com/eric-maynard/riftfound/blob/89622dfd9de088b5898673d8b0dc77573ecaa0ed/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Riftfound

Event calendar aggregator for Riftbound TCG events, scraped from https://locator.riftbound.uvsgames.com/

## Architecture

```
riftfound/
├── backend/     # Express.js API (Lambda + API Gateway)
├── frontend/    # React + Vite calendar UI (S3 + CloudFront)
├── scraper/     # Event scraper (Lambda + EventBridge)
└── infrastructure/  # Terraform, Docker for local dev
```

**Production Stack (Serverless):**
- Frontend: S3 + CloudFront
- Backend API: Lambda + API Gateway (via CloudFront)
- Scraper: Lambda + EventBridge (hourly)
- Database: DynamoDB
- Geocoding: Mapbox Geocoding API v6

## Quick Start

```bash
./dev.sh                    # SQLite mode, no geocoding
./dev.sh --docker           # PostgreSQL only
./dev.sh --docker --photon  # PostgreSQL + Photon geocoder (first run downloads ~8GB)
```

## Key Design Decisions

- **Database**: SQLite for dev, DynamoDB for production. Controlled by `DB_TYPE` env var.
- **Geocoding**: Mapbox API (primary) with public Photon fallback.
- **Shops table**: Stores geocoded locations to avoid re-geocoding. Events reference shops via `shop_id`.
- **Calendar mode**: API returns all events in 3-month window without pagination when `calend
```

</details>
