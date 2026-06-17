---
name: topoteretes__cognee
source: https://github.com/topoteretes/cognee/blob/6c56b29656b28ae15c64a4c3b6cd9069044b569f/CLAUDE.md
repo: topoteretes/cognee
kind: claude-md
stars: 17827
last_pushed: 2026-06-14T21:16:01Z
license: apache-2.0
score: 9
domains: [agents-ai, backend-api, knowledge-graphs]
tags: [architecture-mapping, workflow-driven]
curated: 2026-06-15
curated_by: config-scout
---

# topoteretes/cognee — claude-md

**Why it's worth keeping:** The 'Critical Data Flow Paths' section is a masterclass in teaching an LLM how logic flows through a system; the inclusion of interface patterns provides clear guidance for extending functionality.

**Summary:** Provides deep architectural context by mapping high-level workflows directly to specific file paths and modules. It includes comprehensive setup, testing, and environment configuration details.

**Source credibility:** High popularity (17k+ stars) and active maintenance/recent pushes.

**Recency:** Current, utilizing modern Python tooling like 'uv'.

**Source:** [topoteretes/cognee/CLAUDE.md](https://github.com/topoteretes/cognee/blob/6c56b29656b28ae15c64a4c3b6cd9069044b569f/CLAUDE.md) · 17827★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Cognee is an open-source AI memory platform that transforms raw data into persistent knowledge graphs for AI agents. It replaces traditional RAG (Retrieval-Augmented Generation) with an ECL (Extract, Cognify, Load) pipeline combining vector search, graph databases, and LLM-powered entity extraction.

**Requirements**: Python 3.10 - 3.14

## Development Commands

### Setup
```bash
# Create virtual environment (recommended: uv)
uv venv && source .venv/bin/activate

# Install with pip, poetry, or uv
uv pip install -e .

# Install with dev dependencies
uv pip install -e ".[dev]"

# Install with specific extras
uv pip install -e ".[postgres,neo4j,docs,chromadb]"

# Set up pre-commit hooks
pre-commit install
```

### Available Installation Extras
- **postgres** / **postgres-binary** - PostgreSQL + PGVector support
- **neo4j** - Neo4j graph database support
- **neptune** - AWS Neptune support
- **chromadb** - ChromaDB vector database
- **docs** - Document processing (unstructured library)
- **scraping** - Web scraping (Tavily, BeautifulSoup, Playwright)
```

</details>
