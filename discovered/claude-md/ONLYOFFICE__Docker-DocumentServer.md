---
name: ONLYOFFICE__Docker-DocumentServer
source: https://github.com/ONLYOFFICE/Docker-DocumentServer/blob/1d57f2ba013c3e8743e9d330116b71e728c81df2/CLAUDE.md
repo: ONLYOFFICE/Docker-DocumentServer
kind: claude-md
stars: 2277
last_pushed: 2026-06-15T19:38:21Z
license: agpl-3.0
score: 8
domains: [devops, infrastructure-as-code, docker]
tags: [docker, supervisor, orchestration, deployment]
curated: 2026-06-16
curated_by: config-scout
---

# ONLYOFFICE/Docker-DocumentServer — claude-md

**Why it's worth keeping:** The 'Review Focus' section is excellent—it tells the AI exactly which files contain critical/risky logic (like the entrypoint), and the structured file mapping prevents navigation errors.

**Summary:** Provides a high-level architectural map for a complex Docker-based service orchestration system using Supervisor.

**Source credibility:** High: 2.2k+ stars and highly active maintenance by a reputable organization.

**Recency:** Very current; uses modern Ubuntu 24.04 base and up-to-date Docker patterns.

**Source:** [ONLYOFFICE/Docker-DocumentServer/CLAUDE.md](https://github.com/ONLYOFFICE/Docker-DocumentServer/blob/1d57f2ba013c3e8743e9d330116b71e728c81df2/CLAUDE.md) · 2277★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Project Overview

ONLYOFFICE Docker-DocumentServer — single-container Docker image for ONLYOFFICE Docs with all services (docservice, converter, nginx, PostgreSQL, Redis, RabbitMQ) managed by Supervisor.

## Tech Stack

Docker, Docker BuildX, Bash, Nginx, Supervisor, PostgreSQL/MySQL/MariaDB/MSSQL/Oracle, Redis, RabbitMQ/ActiveMQ

## Project Structure

```
Dockerfile              — Main image (Ubuntu 24.04 base)
production.dockerfile   — Stable/release image builder
docker-compose.yml          — Local dev CE (documentserver only, no bundled services)
docker-compose.enterprise.yml — Local dev EE (with postgres, rabbitmq, redis)
docker-compose.developer.yml  — Local dev DE (with postgres, rabbitmq, redis)
docker-bake.hcl         — BuildX multi-platform config
Makefile                — Build system (image, deploy, clean targets)
run-document-server.sh  — Main entrypoint script (842 lines)
config/supervisor/ds/        — Supervisor service configs (ds, ds-adminpanel, ds-converter, ds-docservice, ds-example, ds-metrics)
config/supervisor/supervisor — Shell script for supervisord startup
tests/                  — Integration tests (DB/AMQP/SSL matrix)
fonts/                  — Custom f
```

</details>
