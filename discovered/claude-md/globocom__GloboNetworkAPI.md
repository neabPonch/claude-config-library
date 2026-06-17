---
name: globocom__GloboNetworkAPI
source: https://github.com/globocom/GloboNetworkAPI/blob/d3edf6820ecf5bad1653dac04eab1ffb231e9546/CLAUDE.md
repo: globocom/GloboNetworkAPI
kind: claude-md
stars: 87
last_pushed: 2026-06-01T19:33:08Z
license: apache-2.0
score: 9
domains: [backend-api, devops]
tags: [django, docker, architecture-patterns, api-design]
curated: 2026-06-14
curated_by: config-scout
---

# globocom/GloboNetworkAPI — claude-md

**Why it's worth keeping:** The explicit 'API Module Pattern' directory tree is an excellent way to teach Claude existing architectural hierarchy. The inclusion of specific 'make' commands reduces trial-and-error for running the environment and tests.

**Summary:** Provides comprehensive technical context including Docker-based dev workflows and specific test execution patterns. It outlines a sophisticated API module pattern that explains where logic resides versus views.

**Source credibility:** High: Globo is a major tech/media entity, and the repo shows active maintenance history.

**Recency:** The tech stack is legacy (Python 2.7), but the documentation structure is highly compatible with modern agentic workflows.

**Source:** [globocom/GloboNetworkAPI/CLAUDE.md](https://github.com/globocom/GloboNetworkAPI/blob/d3edf6820ecf5bad1653dac04eab1ffb231e9546/CLAUDE.md) · 87★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

GloboNetworkAPI is a REST API for managing IP networking resources (VLAN, IP, Network, Equipment, VIP, etc.). Built with Django 1.5 and Python 2.7, running on MySQL with Memcached, Celery/RabbitMQ for async tasks.

## Development Environment

All development runs inside Docker containers via docker-compose.

```bash
# Start all services (MySQL, RabbitMQ, Memcached, Celery, NetAPI)
make start

# Stop all services
make stop

# Shell into app container
make api

# Shell into database container
make db

# View logs
make logs

# Build Docker images
make build_img
```

## Running Tests

Tests run inside the Docker container. The test settings module is `networkapi.settings_ci`.

```bash
# Full test suite (fresh DB each run)
make test_ci

# Full test suite (reuses DB, faster)
make test

# Specific app tests
make test_ci app=networkapi/api_vlan
make test app=networkapi/plugins/SDN/

# Single test module from inside the container
docker exec -it netapi_app ./fast_start_test_reusedb.sh networkapi/api_vlan
```

Test runner uses `python manage.py test` with
```

</details>
