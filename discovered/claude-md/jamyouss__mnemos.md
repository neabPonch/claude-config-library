---
name: jamyouss__mnemos
source: https://github.com/jamyouss/mnemos/blob/ec93036230ad3197856c49c47b04a5ec17188237/CLAUDE.md
repo: jamyouss/mnemos
kind: claude-md
stars: 0
last_pushed: 2026-05-28T14:51:03Z
license: mit
score: 9
domains: [agents-ai, backend-api, cli-tools]
tags: [rag, mcp, python, qdrant]
curated: 2026-06-14
curated_by: config-scout
---

# jamyouss/mnemos — claude-md

**Why it's worth keeping:** The 'When to intervene' section is elite; it enforces architectural guardrails like 'single source of truth' for path filters. It also provides exact command sequences for re-indexing, which is crucial for maintaining the system's state.

**Summary:** A highly technical blueprint for a RAG-powered memory layer that explains data pipelines, vector scoping via tags, and MCP toolsets.

**Source credibility:** Low star count, but the extreme technical density and specific architecture details suggest a highly capable author.

**Recency:** Very current; leverages modern standards like MCP and Python 3.12.

**Source:** [jamyouss/mnemos/CLAUDE.md](https://github.com/jamyouss/mnemos/blob/ec93036230ad3197856c49c47b04a5ec17188237/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Mnemos — Claude Code Instructions

> Self-hosted memory layer for AI coding agents. Indexes codebase + docs + skills, extracts memories from git, exposes everything via MCP.

## Mission

Mnemos est un **RAG dev-centric self-hosted** qui sert de couche mémoire pour les agents AI (Claude Code, Claude Desktop). Il combine :
- **Code retrieval** : indexing AST-aware (Go via tree-sitter, Vue SFC, Markdown)
- **Memory pipeline** : extraction automatique depuis git, dedup LLM, workflow d'approbation
- **Agent context** : indexing des skills Claude et docs d'architecture

Exposé comme MCP server (Streamable HTTP) sur `localhost:8100/mcp`.

## Architecture

### Pipeline RAG actuel

```
INDEXING (watcher / push API / CLI):
  file → chunker (par extension) → embedder → Qdrant upsert
         AST Go (tree-sitter) | Vue SFC | MD headings | Fallback
         all-MiniLM-L6-v2 (384 dims, cosine, normalized)

RETRIEVAL (MCP / REST):
  query → embed → query_points(N collections séquentiel) → sort by score → top-K
         ⚠️ Pas de reranker, pas de hybrid, pas de query router

MEMORY (git hook / API):
  git commit → Ollama extract decisions/patterns/lessons →
  dedup (cos sim ≥ 0.85, merge ou repl
```

</details>
