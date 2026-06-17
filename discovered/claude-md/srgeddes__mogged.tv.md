---
name: srgeddes__mogged.tv
source: https://github.com/srgeddes/mogged.tv/blob/c04df103b2fd693089e15de7d12d95b15a936c63/claude.md
repo: srgeddes/mogged.tv
kind: claude-md
stars: 0
last_pushed: 2026-03-20T03:10:46Z
license: unknown
score: 9
domains: [backend-api, web-frontend, fullstack]
tags: [DDD, FastAPI, React, Tailwind, Architecture]
curated: 2026-06-14
curated_by: config-scout
---

# srgeddes/mogged.tv — claude-md

**Why it's worth keeping:** The directory tree uses functional annotations to explain file roles; the semantic color token table is an elite way to guide visual styling through AI; and it enforces strict separation of concerns between routers, services, and repositories.

**Summary:** A high-quality full-stack instruction set using Domain-Driven Design (DDD) and strict architectural layers. It includes a specific semantic color system for UI consistency.

**Source credibility:** Low GitHub social proof, but high technical density (uv, Pydantic v2, SQLAlchemy 2.0) indicates a professional-grade developer setup.

**Recency:** Extremely current, utilizing modern tools like Python 3.12, uv, and the latest Pydantic/SQLAlchemy versions.

**Source:** [srgeddes/mogged.tv/claude.md](https://github.com/srgeddes/mogged.tv/blob/c04df103b2fd693089e15de7d12d95b15a936c63/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# claude.md — mogged.tv

## Project overview

mogged.tv is a private, self-hosted live streaming platform for small groups. It uses LiveKit for real-time video/audio/chat, FastAPI for the backend API, React for the frontend, and PostgreSQL for persistence. Target scale is 1-10 concurrent viewers per stream.

## Technology stack

- Python 3.12, FastAPI, SQLAlchemy 2.0 (async), Pydantic v2, Alembic
- React 18+ with TypeScript
- LiveKit (self-hosted, WebRTC)
- PostgreSQL 16
- Redis (caching, optional)
- Docker / Docker Compose
- uv package manager
- Ruff for linting and formatting
- pytest + pytest-asyncio for testing

## Architecture

Domain-Driven Design. Code is organized by domain, not by technical layer.

Three main pieces:

1. **LiveKit server** — handles all real-time media (video, audio, screen share, chat via data channels). Runs as a Docker container on the VPS.
2. **FastAPI backend** — handles auth, user management, stream metadata, and generates LiveKit access tokens. This is the gatekeeper — LiveKit trusts whatever tokens the backend signs.
3. **React frontend** — the UI. Uses LiveKit's React SDK for the stream/chat view and talks to the FastAPI backend for everything els
```

</details>
