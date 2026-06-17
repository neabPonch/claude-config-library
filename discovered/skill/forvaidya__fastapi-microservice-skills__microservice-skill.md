---
name: forvaidya__fastapi-microservice-skills__microservice-skill
source: https://github.com/forvaidya/fastapi-microservice-skills/blob/b796e2902831d76ec061bdf5290f646b84d27918/MICROSERVICE_SKILL.md
repo: forvaidya/fastapi-microservice-skills
kind: skill
stars: 0
last_pushed: 2026-03-03T14:13:13Z
license: unknown
score: 8
domains: [backend-api, microservices, architecture-patterns]
tags: [fastapi, redis, rule-engine]
curated: 2026-06-16
curated_by: config-scout
---

# forvaidya/fastapi-microservice-skills — skill

**Why it's worth keeping:** The explicit distinction between global and service-scoped rules, paired with the detailed lifecycle stages, provides high-density structural constraints for an agent to follow.

**Summary:** A blueprint for building event-driven microservices using a centralized rule engine and Redis Pub/Sub.

**Source credibility:** Low-star personal repository containing highly dense technical specifications.

**Recency:** Very current; aligns with modern FastAPI and asynchronous Python patterns.

**Source:** [forvaidya/fastapi-microservice-skills/MICROSERVICE_SKILL.md](https://github.com/forvaidya/fastapi-microservice-skills/blob/b796e2902831d76ec061bdf5290f646b84d27918/MICROSERVICE_SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Microservice Skill: Rule-Based Distributed System

**Version:** 1.0
**Pattern:** Separation of Concerns with Redis-backed Rule Engine
**Languages:** Python (FastAPI, asyncio)
**Use Case:** Build event-driven microservices with centralized rule management

---

## Overview

This skill teaches Claude Code to scaffold and work with a **microservice architecture** where:
- **Configurator** manages rules/config (CRUD) via REST API
- **Microservices** fetch and execute rules independently
- **Redis** stores rules and config, broadcasts changes via Pub/Sub
- **Shared libraries** (outside microservices) provide common utilities

### Key Pattern
**Separation of Concerns:**
- Rules management ≠ Rule execution
- Config centralized ≠ Config pushed (pull model)
- Global rules (service: "*") execute on ALL services
- Service-scoped rules (service: "my-service") execute on one service

---

## Architecture at a Glance

```
┌─────────────────────────────────────────────┐
│         CONFIGURATOR (Port :8002)           │
│  • CRUD Rules                               │
│  • Manage Config                            │
│  • Publish changes to Redis Pub/Sub          │
└──────────────┬───────────────────
```

</details>
