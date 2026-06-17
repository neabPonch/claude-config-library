---
name: Code-and-Learn-with-AI__weather-fast-api-agentic
source: https://github.com/Code-and-Learn-with-AI/weather-fast-api-agentic/blob/af30d277c86243f930d2381af13518c456718bc1/Claude.md
repo: Code-and-Learn-with-AI/weather-fast-api-agentic
kind: claude-md
stars: 0
last_pushed: 2026-04-18T05:29:10Z
license: unknown
score: 8
domains: [backend-api, python]
tags: [fastapi, tdd, architecture, uv]
curated: 2026-06-15
curated_by: config-scout
---

# Code-and-Learn-with-AI/weather-fast-api-agentic — claude-md

**Why it's worth keeping:** It includes essential 'negative constraints' (e.g., no silent edits or speculative code) and uses Mermaid diagrams to provide the LLM with spatial/topological context.

**Summary:** A highly structured operational manual that defines strict TDD workflows and clear architectural boundaries for an AI agent.

**Source credibility:** Low star count suggests a personal pedagogical project, but the technical structure is professional.

**Recency:** 

**Source:** [Code-and-Learn-with-AI/weather-fast-api-agentic/Claude.md](https://github.com/Code-and-Learn-with-AI/weather-fast-api-agentic/blob/af30d277c86243f930d2381af13518c456718bc1/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude.md

Living document for Claude-assisted work on this project. Updated at the end of every phase.

## 1. Project purpose

Weather queries by city name, served via a FastAPI backend and a Streamlit frontend.
Results are persisted in Postgres and cached in Redis. Built TDD-first, incrementally.

## 2. Architecture overview

- **`app/core/config.py`** — Pydantic `Settings` loaded from environment variables.
- **`app/core/logging.py`** — JSON structured logging via stdlib; `setup_logging()` configures the root logger.
- **`app/main.py`** — FastAPI app instance with `RequestIDMiddleware` and the `/health` endpoint.
- **`app/routers/`** — one router per feature (e.g. `weather.py`). Registered on `app` at startup.
- **`app/schemas/`** — Pydantic request/response models.
- **`app/services/`** — business logic; orchestrates external clients, cache, repositories.
- **`app/repositories/`** — database access via SQLAlchemy async.
- **`app/models/`** — SQLAlchemy ORM models.

## 3. Folder tree

```
weather-fast-api-agentic/
├── app/
│   ├── core/
│   │   ├── config.py        # Pydantic Settings
│   │   └── logging.py       # JSON log setup
│   ├── models/              # ORM models (Phas
```

</details>
