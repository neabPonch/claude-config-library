---
name: morphik-org__morphik-core
source: https://github.com/morphik-org/morphik-core/blob/03a93e89acc801049b887b1b8e974110ddc728db/CLAUDE.md
repo: morphik-org/morphik-core
kind: claude-md
stars: 3611
last_pushed: 2026-05-11T02:18:12Z
license: other
score: 9
domains: [backend-api, ai-agents, fullstack]
tags: [python, fastapi, nextjs, rag, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# morphik-org/morphik-core — claude-md

**Why it's worth keeping:** The 'Key Components and Patterns' section provides semantic context about the system logic rather than just folder locations. It also explicitly lists specific tooling like `uv` and `ruff`, which enables more precise command generation.

**Summary:** Provides a comprehensive architectural map and clear execution instructions for both Python backend and Next.js frontend.

**Source credibility:** High; the repository is highly starred (3611) and shows recent maintenance.

**Recency:** Very current, reflecting modern toolchains such as `uv` and Next.js.

**Source:** [morphik-org/morphik-core/CLAUDE.md](https://github.com/morphik-org/morphik-core/blob/03a93e89acc801049b887b1b8e974110ddc728db/CLAUDE.md) · 3611★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Morphik is an AI-native toolset for visually rich documents and multimodal data. It provides end-to-end RAG (Retrieval-Augmented Generation) capabilities for processing, storing, and querying unstructured documents with advanced multimodal search capabilities including ColPali.

## Architecture

### Backend (Python)
- **Core API**: Located in `/core` - FastAPI-based REST API
- **Database**: PostgreSQL with pgvector for vector similarity search
- **Models**: SQLAlchemy models in `core/models/`
- **Services**: Business logic in `core/services/`
- **Routes**: API endpoints in `core/routes/`
- **Vector Store**: Multiple providers (pgvector, TurboPuffer) in `core/vector_store/`
- **Embedding**: Support for multiple providers (OpenAI, Ollama, Azure) in `core/embedding/`
- **Parser**: Document processing and chunking in `core/parser/`

### Frontend (TypeScript/Next.js)
- **Location**: `ee/ui-component/` - Enterprise Edition UI component
- **Tech Stack**: Next.js, TypeScript, ShadCN UI components, Tailwind CSS
- **Purpose**: Web interface for document up
```

</details>
