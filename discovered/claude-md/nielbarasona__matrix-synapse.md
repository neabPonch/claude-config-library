---
name: nielbarasona__matrix-synapse
source: https://github.com/nielbarasona/matrix-synapse/blob/ff2cb36fd4085af71a4829c5e591b20c673f84e1/CLAUDE.md
repo: nielbarasona/matrix-synapse
kind: claude-md
stars: 1
last_pushed: 2026-02-12T03:07:07Z
license: unknown
score: 9
domains: [devops, infrastructure-as-code, self-hosting]
tags: [docker, matrix, deployment, iac]
curated: 2026-06-16
curated_by: config-scout
---

# nielbarasona/matrix-synapse — claude-md

**Why it's worth keeping:** The ASCII architecture diagram provides essential network context, while the 'Key Constraints' section preemptively addresses critical configuration pitfalls like secret matching and syntax sensitivity.

**Summary:** A highly effective guide for managing infrastructure-as-code via Docker Compose, focusing on deployment orchestration and configuration mapping.

**Source credibility:** Niche/specialized repository with specific technical depth despite low star count.

**Recency:** 

**Source:** [nielbarasona/matrix-synapse/CLAUDE.md](https://github.com/nielbarasona/matrix-synapse/blob/ff2cb36fd4085af71a4829c5e591b20c673f84e1/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Docker Compose deployment configuration for a self-hosted Matrix Synapse homeserver. This is **not** a software library — it's infrastructure-as-code with no build step, test suite, or linting.

## Commands

```bash
# Start/stop all services
docker compose up -d
docker compose down

# View logs
docker compose logs -f [synapse|caddy|postgres|element|coturn]

# Update images
docker compose pull && docker compose up -d

# Create admin user
docker compose exec synapse register_new_matrix_user \
  -c /data/homeserver.yaml -u admin -a http://localhost:8008

# Backup/restore database
docker compose exec postgres pg_dump -U synapse synapse > backup.sql
cat backup.sql | docker compose exec -T postgres psql -U synapse synapse
```

## Architecture

```
Internet
  ├─ :80/:443/:8448 ──► Caddy (TLS termination, auto Let's Encrypt)
  │                        ├─► Synapse (:8008) ──► PostgreSQL
  │                        ├─► Element Web (:80)
  │                        ├─► lk-jwt-service (:8080)  [livekit subdomain]
  │                        └─► LiveKit (:7880)
```

</details>
