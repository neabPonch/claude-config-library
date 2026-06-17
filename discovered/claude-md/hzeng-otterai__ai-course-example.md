---
name: hzeng-otterai__ai-course-example
source: https://github.com/hzeng-otterai/ai-course-example/blob/cd8fb4681b423133aaf9453ff09c81949362629f/CLAUDE.md
repo: hzeng-otterai/ai-course-example
kind: claude-md
stars: 11
last_pushed: 2026-05-03T00:38:22Z
license: apache-2.0
score: 8
domains: [agents-ai, backend-api, web-fullstack]
tags: [educational, agentic-patterns, rag, python]
curated: 2026-06-15
curated_by: config-scout
---

# hzeng-otterai/ai-course-example — claude-md

**Why it's worth keeping:** It provides explicit implementation details for agentic tool loops and API nuances, which helps Claude maintain logic consistency when modifying code rather than just following basic file structures.

**Summary:** A highly structured guide that combines execution commands with deep architectural pattern documentation.

**Source credibility:** Solid educational repository with a respectable star count and recent activity.

**Recency:** Very current; includes modern tech like React 19 and specific Anthropic SDK patterns.

**Source:** [hzeng-otterai/ai-course-example/CLAUDE.md](https://github.com/hzeng-otterai/ai-course-example/blob/cd8fb4681b423133aaf9453ff09c81949362629f/CLAUDE.md) · 11★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Purpose

Educational examples for building chatbots and AI agents with LLMs, organized as independent modules demonstrating progressive complexity: direct API usage → LangChain framework → full-stack apps → agentic loops.

## Running Code

All modules are standalone Python scripts. Run them directly:

```bash
python backend_api/test_chat_simple.py
python backend_langchain/test_05_rag.py
python ai_agent/test_loop_agent.py
python embedding_test/run_embedding_search.py
```

**Required environment variables** (`.env` file):
- `OPENAI_API_KEY` (for `backend_api/`, `backend_langchain/`, `fullstack_flask/`)
- `ANTHROPIC_API_KEY` (for `ai_agent/`)
- `PINECONE_API_KEY` (for Pinecone examples)
- `TAVILY_API_KEY` (for `ai_agent/test_chat_with_rag.py`)

### fullstack_flask app

```bash
pip install -r fullstack_flask/requirements.txt

# Initialize DB (first time only)
python -c "from src.app import app, db; app.app_context().__enter__(); db.create_all()"

gunicorn src.app:app        # http://localhost:50505
docker-compose up           # alternatively
```

### notebook_app_by_c
```

</details>
