---
name: bunkerity__bunkerweb
source: https://github.com/bunkerity/bunkerweb/blob/515efe94ab3982e6ab01768fb1ff46d3871c1b95/CLAUDE.md
repo: bunkerity/bunkerweb
kind: claude-md
stars: 10622
last_pushed: 2026-06-12T15:35:45Z
license: agpl-3.0
score: 9
domains: [security, backend-api, infrastructure]
tags: [architecture-map, workflow-driven, devops]
curated: 2026-06-15
curated_by: config-scout
---

# bunkerity/bunkerweb — claude-md

**Why it's worth keeping:** The 'Configuration Flow' section explains state transitions rather than just file lists, and the mapping of core components to their functional roles allows Claude to reason about side effects. The inclusion of specific linting/formatting toolsets makes it highly actionable for code quality maintenance.

**Summary:** Provides an exhaustive architectural blueprint of a complex WAF system, detailing component interactions and the specific logic of configuration flows.

**Source credibility:** High; sourced from a popular (10k+ stars) and actively maintained security project.

**Recency:** Current; reflects modern development workflows including containerized environments and specific linting standards.

**Source:** [bunkerity/bunkerweb/CLAUDE.md](https://github.com/bunkerity/bunkerweb/blob/515efe94ab3982e6ab01768fb1ff46d3871c1b95/CLAUDE.md) · 10622★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

BunkerWeb is an open-source Web Application Firewall (WAF) built on NGINX with a modular plugin architecture. It provides "security by default" for web services through multiple integration modes (Docker, Kubernetes, Swarm, Linux) and is fully configurable via environment variables.

## Architecture

### Core Components

- **BunkerWeb Core** (`src/bw/`, `src/common/core/`): NGINX-based reverse proxy with security modules in Lua (request-time) and Python (jobs). Entry point: `src/bw/lua/bunkerweb.lua`.
- **Scheduler** (`src/scheduler/`): Central orchestrator ("brain"). `main.py` runs the main loop; `JobScheduler.py` manages job execution with thread pools. Uses Python's `schedule` library.
- **Autoconf** (`src/autoconf/`): Listens for Docker/Swarm/Kubernetes events and dynamically reconfigures BunkerWeb.
- **API** (`src/api/`): FastAPI service with router-based architecture (`src/api/app/routers/` — auth, instances, services, configs, plugins, jobs). IP whitelist and rate limiting support.
- **Web UI** (`src/ui/`): Flask app using Blueprints for r
```

</details>
