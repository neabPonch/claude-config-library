---
name: erick-mb__vehicles_fleet_api_project__backend-skill
source: https://github.com/erick-mb/vehicles_fleet_api_project/blob/0f464af8e7787a508e0f10b035c333ba55a1728f/skills/backend-skill.md
repo: erick-mb/vehicles_fleet_api_project
kind: skill
stars: 0
last_pushed: 2026-02-16T15:43:02Z
license: unknown
score: 8
domains: [backend-api, python]
tags: [fastapi, mongodb, architecture, layering]
curated: 2026-06-16
curated_by: config-scout
---

# erick-mb/vehicles_fleet_api_project — skill

**Why it's worth keeping:** It provides specific, high-level structural patterns like ABC interfaces and the Pipeline pattern, plus actionable rules for error logging and database access strategy.

**Summary:** A comprehensive architectural blueprint for building FastAPI services with MongoDB using a layered approach.

**Source credibility:** Low social proof (0 stars), but the content represents professional-grade architectural standards.

**Recency:** Highly current, specifying Python 3.11+ and modern FastAPI patterns.

**Source:** [erick-mb/vehicles_fleet_api_project/skills/backend-skill.md](https://github.com/erick-mb/vehicles_fleet_api_project/blob/0f464af8e7787a508e0f10b035c333ba55a1728f/skills/backend-skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: backend-fastapi-mongodb
description: Backend API development standards for Fleet Management. Use for creating FastAPI endpoints, MongoDB operations, error handling, validation, and service logic.
---

# Backend Development Standards (FastAPI + MongoDB)

## Technology Stack
- **Framework:** FastAPI 0.104.1+
- **Database:** MongoDB with pymongo (NOT motor)
- **Python:** 3.11+
- **Async:** Built-in to FastAPI, used for I/O operations
- **Containerization:** Docker + Docker Compose

## Architecture Patterns

### Layered Architecture (Modular)
The codebase follows a strict 4-layer architecture for maximum clarity and testability:

```
HTTP Request
    ↓
Routes Layer (HTTP handling)
    ↓
Service Layer (Business logic)
    ↓
Repository Layer (Data access)
    ↓
MongoDB
```

**Why this pattern:**
- Each layer has a single responsibility
- Easy to test each layer independently
- Clear data flow (debuggable)
- Reusable components across endpoints

### ABC Pattern for Interfaces
Use Python's `ABC` (Abstract Base Class) for defining component contracts:
- Define interfaces with abstract methods in base classes
- Prevents code duplication
- Enforces consistent method signatures
- Exa
```

</details>
