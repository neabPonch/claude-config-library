---
name: TryGhost__ghost-docker
source: https://github.com/TryGhost/ghost-docker/blob/07dac00e1bf2340b5b731b2147ecad89fd14f2a1/CLAUDE.md
repo: TryGhost/ghost-docker
kind: claude-md
stars: 90
last_pushed: 2026-06-13T23:35:20Z
license: mit
score: 8
domains: [devops, cms, docker]
tags: [ghost-cms, docker-compose, deployment]
curated: 2026-06-15
curated_by: config-scout
---

# TryGhost/ghost-docker — claude-md

**Why it's worth keeping:** It provides high-density operational intelligence, such as exact env var naming conventions and profile-specific startup commands, which are crucial for an agent's tool use.

**Summary:** Defines service architecture, environment variable schemas, and specific Docker Compose command patterns including profiles.

**Source credibility:** High; the repo is active and well-maintained with 90 stars.

**Recency:** Current; follows modern Docker Compose standards.

**Source:** [TryGhost/ghost-docker/CLAUDE.md](https://github.com/TryGhost/ghost-docker/blob/07dac00e1bf2340b5b731b2147ecad89fd14f2a1/CLAUDE.md) · 90★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a comprehensive Docker Compose setup for running Ghost CMS in production with automatic HTTPS, optional analytics, and ActivityPub support. The repository orchestrates multiple services including Ghost, MySQL, Caddy (reverse proxy), and optional Tinybird analytics and ActivityPub federation.

## Architecture

The project uses Docker Compose to orchestrate these services:

1. **Ghost** - The main CMS application (runs on internal port 2368)
2. **MySQL** - Database backend with health checks and support for multiple databases
3. **Caddy** - Reverse proxy handling HTTPS/SSL, routing, and external access
4. **Traffic Analytics** (optional profile) - Tinybird integration for web analytics
5. **ActivityPub** (optional profile) - Federated social networking support
6. **Supporting services** - Tinybird setup tools and ActivityPub migrations

Services communicate internally via Docker networks. Caddy handles all external traffic routing including special paths for analytics (`/_tinybird`) and ActivityPub (`/.well-known/`, `/activitypub/`).

## Co
```

</details>
