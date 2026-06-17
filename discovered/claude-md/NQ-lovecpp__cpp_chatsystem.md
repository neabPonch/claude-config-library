---
name: NQ-lovecpp__cpp_chatsystem
source: https://github.com/NQ-lovecpp/cpp_chatsystem/blob/c1fccf920993ac09446702035e7ff17984cbfe0d/CLAUDE.md
repo: NQ-lovecpp/cpp_chatsystem
kind: claude-md
stars: 6
last_pushed: 2026-05-18T04:50:10Z
license: unknown
score: 9
domains: [microservices, ai-agents, fullstack-development]
tags: [architecture-mapping, event-driven, multi-language, data-flow]
curated: 2026-06-16
curated_by: config-scout
---

# NQ-lovecpp/cpp_chatsystem — claude-md

**Why it's worth keeping:** The 'Data Flow' section and granular module descriptions allow an AI to understand cross-service side effects. It also maps specific event types and port mappings essential for debugging distributed state.

**Summary:** A high-density architectural map of a complex, multi-language microservices system covering C++, Python (AI Agents), and React.

**Source credibility:** A specialized real-time communication project with decent structure despite lower star count.

**Recency:** 

**Source:** [NQ-lovecpp/cpp_chatsystem/CLAUDE.md](https://github.com/NQ-lovecpp/cpp_chatsystem/blob/c1fccf920993ac09446702035e7ff17984cbfe0d/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A hybrid chat system with two backends:
- **C++ Microservices** (`ChatSystem-Backend/`): 7 domain services + API gateway, built with brpc, protobuf, Redis, MySQL, etcd, RabbitMQ
- **Python Agent Server** (`ChatSystem-Backend/8.Agent_Server/`): FastAPI + OpenAI Agents SDK, provides AI assistant functionality
- **React Frontend** (`ChatSystem-Frontend-React/`): Ant Design X UI, communicates with both backends

## Development Commands

### Agent Server (Python)
```bash
cd ChatSystem-Backend/8.Agent_Server
source /home/chen/cpp_chatsystem/.venv/bin/activate  # 或: uv sync 后使用 uv run
uvicorn src.main:app --host 0.0.0.0 --port 8080 --reload
```
环境：工作区使用 uv + Python 3.12，详见 `8.Agent_Server/PYTHON_SETUP.md`

### React Frontend
```bash
cd ChatSystem-Frontend-React
npm install
npm run dev        # Dev server on port 5173
npm run build      # Production build
npm run preview    # Preview production build
```

### Infrastructure (Docker)
```bash
cd ChatSystem-Backend
docker-compose up -d    # Start all infrastructure services
docker-compose down     # Stop se
```

</details>
