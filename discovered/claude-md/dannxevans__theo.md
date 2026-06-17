---
name: dannxevans__theo
source: https://github.com/dannxevans/theo/blob/b8ee751747a5fc6248a295ce598382f27a0737d2/CLAUDE.MD
repo: dannxevans/theo
kind: claude-md
stars: 2
last_pushed: 2026-01-17T13:02:16Z
license: unknown
score: 8
domains: [agents-ai, backend-api]
tags: [agentic-workflows, architecture-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# dannxevans/theo — claude-md

**Why it's worth keeping:** It explains systemic behaviors like circuit breakers and data lifecycles, which helps an AI understand how individual changes impact the broader system state.

**Summary:** Provides deep architectural context for complex agentic workflows, including intent routing and a multi-module memory system.

**Source credibility:** Small personal project with high technical density in documentation.

**Recency:** Highly current; reflects modern agentic design patterns despite a likely typo in the future-dated roadmap.

**Source:** [dannxevans/theo/CLAUDE.MD](https://github.com/dannxevans/theo/blob/b8ee751747a5fc6248a295ce598382f27a0737d2/CLAUDE.MD) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.MD - AI Assistant Guide for THEO

This document provides context for AI assistants (like Claude) working on the THEO codebase.

## Project Overview

THEO is a self-hosted personal AI assistant that intelligently routes requests to the most appropriate AI model based on intent, while maintaining conversation continuity and context across models.

**Philosophy**: Not "one model to rule them all" - use different models for different tasks while preserving seamless user experience.

## Tech Stack

- **Backend**: Python 3.9+ with Flask
- **Frontend**: Svelte 4 with Vite 5
- **Database**: SQLite with SQLAlchemy ORM
- **Real-time Communication**: Socket.IO with Flask-SocketIO
- **Authentication**: Session tokens + API keys (bcrypt hashing)
- **Testing**: pytest (backend), coverage tracking
- **Deployment**: Docker, AWS ECS (historical)

## Project Structure

```
theo/
├── dev-docs/                       # Implementation plans for active development
├── backend/
│   ├── app.py                      # Main Flask application entry point
│   ├── config.py                   # Configuration management
│   ├── requirements.txt            # Python dependencies
│   │
│   ├── routes/
```

</details>
