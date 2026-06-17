---
name: 77z-zhou__graph_builder
source: https://github.com/77z-zhou/graph_builder/blob/b106d1957778893de1fbcc7bf4d3b19725b463be/CLAUDE.md
repo: 77z-zhou/graph_builder
kind: claude-md
stars: 6
last_pushed: 2026-01-30T09:58:09Z
license: unknown
score: 9
domains: [backend-api, agents-ai, knowledge-graphs, data-engineering]
tags: [fastapi, neo4j, langchain, rag]
curated: 2026-06-16
curated_by: config-scout
---

# 77z-zhou/graph_builder — claude-md

**Why it's worth keeping:** The explicit Graph Schema (nodes/relationships) and the layered directory breakdown are perfect for allowing an LLM to write accurate Cypher queries and understand module dependencies without manual exploration.

**Summary:** A highly detailed guide that explains the technical architecture, specific graph database schemas, and multi-stage processing workflows.

**Source credibility:** Respectable niche project with 6 stars and recent maintenance history.

**Recency:** Highly current, utilizing modern tech stacks like FastAPI, Pydantic, and LangChain/LangGraph.

**Source:** [77z-zhou/graph_builder/CLAUDE.md](https://github.com/77z-zhou/graph_builder/blob/b106d1957778893de1fbcc7bf4d3b19725b463be/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **Knowledge Graph Builder** - a Python FastAPI backend system that extracts knowledge graphs from documents using LLMs (Large Language Models) and stores them in Neo4j graph database. The system processes documents in chunks, extracts entities and relationships using LLMs, generates embeddings, and creates a searchable graph knowledge base.

**Core workflow:** Upload file → Chunk document → Extract entities/relationships with LLM → Generate embeddings → Store in Neo4j

## Technology Stack

- **Backend Framework:** FastAPI (async Python web framework)
- **Database:** Neo4j graph database
- **LLM Integration:** LangChain framework
  - Supported LLMs: DeepSeek (`deepseek-chat`), Alibaba Qwen (`qwen3-max` via DashScope)
- **Embeddings:** Qwen/Qwen3-Embedding-0.6B (sentence transformers), HuggingFace embeddings
- **Document Processing:** PyMuPDF (PDF), Unstructured (multi-format loader)
- **API Design:** RESTful with async/await, Pydantic validation

## Architecture

The codebase follows a **layered architecture** pattern:

```
backend/
├──
```

</details>
