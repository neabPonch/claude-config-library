---
name: airweave-ai__airweave
source: https://github.com/airweave-ai/airweave/blob/1ebe1af2dbfb90f3334410721e69997e4f02b320/CLAUDE.md
repo: airweave-ai/airweave
kind: claude-md
stars: 6446
last_pushed: 2026-06-05T09:52:19Z
license: mit
score: 9
domains: [backend-api, web-frontend, ai-agents, data-engineering]
tags: [monorepo, fastapi, react, architecture-map]
curated: 2026-06-15
curated_by: config-scout
---

# airweave-ai/airweave — claude-md

**Why it's worth keeping:** It includes high-value 'contracts' like the OAuth flow and explains unique identifier conventions (short_name) which prevent logical errors. The use of directory trees and specific test markers provides excellent spatial and operational context for an AI.

**Summary:** A comprehensive technical manual for a complex monorepo that covers architecture, command-line workflows, and specific business logic patterns.

**Source credibility:** Highly credible; 6k+ stars, active development as of this month, and professional-grade technical depth.

**Recency:** Very current; uses modern stacks like Python 3.13, Vite, and ShadCN.

**Source:** [airweave-ai/airweave/CLAUDE.md](https://github.com/airweave-ai/airweave/blob/1ebe1af2dbfb90f3334410721e69997e4f02b320/CLAUDE.md) · 6446★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What is Airweave?

Airweave is an open-source platform that makes any app searchable for AI agents by syncing data from 50+ sources into vector databases. It serves as a context retrieval layer for RAG systems and AI agents.

## Architecture

Monorepo with four main components:
- **Backend** (`backend/`): Python 3.13, FastAPI, SQLAlchemy async, PostgreSQL
- **Frontend** (`frontend/`): React 18, TypeScript, Vite, ShadCN UI, TailwindCSS
- **Workers**: Temporal for async sync orchestration, Redis for pub/sub
- **MCP Server** (`mcp/`): Node.js, Streamable HTTP transport for AI assistant integration

Data flow: Sources → Entity extraction → Transformation (DAG) → Embedding → Vector DB → Agent queries

## Common Commands

### Local Development (Docker)
```bash
./start.sh                     # Start all services
./start.sh --skip-frontend     # Backend only
./start.sh --restart           # Restart services
./start.sh --destroy           # Tear down everything
```

### Backend
```bash
cd backend
poetry install                 # Install dependencies
poetry run uvicorn airw
```

</details>
