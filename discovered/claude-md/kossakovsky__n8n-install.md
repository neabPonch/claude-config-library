---
name: kossakovsky__n8n-install
source: https://github.com/kossakovsky/n8n-install/blob/6b223b89648511a1df779e2c60fdd6cc88f62add/CLAUDE.md
repo: kossakovsky/n8n-install
kind: claude-md
stars: 886
last_pushed: 2026-05-17T18:41:18Z
license: apache-2.0
score: 9
domains: [devops, cli-tools, infrastructure]
tags: [docker-compose, automation, system-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# kossakovsky/n8n-install — claude-md

**Why it's worth keeping:** The 'Adding a New Service' section is a perfect example of providing a multi-step, cross-file recipe that ensures consistency when an agent modifies complex infrastructure.

**Summary:** This file provides a comprehensive architectural map and a strict procedural workflow for extending the system with new services. It connects high-level commands (Makefile) to specific backend orchestration logic.

**Source credibility:** High; the repository has strong community interest (886 stars) and active maintenance.

**Recency:** Very recent; last pushed 1 month ago.

**Source:** [kossakovsky/n8n-install/CLAUDE.md](https://github.com/kossakovsky/n8n-install/blob/6b223b89648511a1df779e2c60fdd6cc88f62add/CLAUDE.md) · 886★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is **n8n-install**, a Docker Compose-based installer that provides a comprehensive self-hosted environment for n8n workflow automation and numerous AI/automation services. The installer includes an interactive wizard, automated secret generation, and integrated HTTPS via Caddy.

### Core Architecture

- **Profile-based service management**: Services are activated via Docker Compose profiles (e.g., `n8n`, `flowise`, `monitoring`). Profiles are stored in the `.env` file's `COMPOSE_PROFILES` variable.
- **No exposed ports**: Services do NOT publish ports directly. All external HTTPS access is routed through Caddy reverse proxy on ports 80/443.
- **Shared secrets**: Core services (Postgres, Valkey (Redis-compatible, container named `redis` for backward compatibility), Caddy) are always included. Other services are optional and selected during installation.
- **Queue-based n8n**: n8n runs in `queue` mode with Redis, Postgres, and dynamically scaled workers (`N8N_WORKER_COUNT`).

### Key Files

- `Makefile`: Common commands (install, update, logs,
```

</details>
