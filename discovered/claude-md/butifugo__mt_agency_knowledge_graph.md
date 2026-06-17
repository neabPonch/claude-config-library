---
name: butifugo__mt_agency_knowledge_graph
source: https://github.com/butifugo/mt_agency_knowledge_graph/blob/f0a5d919d4a326f185512f11becd54079d9e34c6/CLAUDE.md
repo: butifugo/mt_agency_knowledge_graph
kind: claude-md
stars: 0
last_pushed: 2026-06-05T15:03:01Z
license: unknown
score: 9
domains: [data-engineering, knowledge-graphs, ai-agents, cli-tools]
tags: [rag, graph-engine, mcp, pipeline]
curated: 2026-06-15
curated_by: config-scout
---

# butifugo/mt_agency_knowledge_graph — claude-md

**Why it's worth keeping:** It utilizes a 'Rules to honor' section to establish strict architectural contracts (schema-first and single source of truth) and provides exhaustive command sets for all development phases.

**Summary:** A sophisticated data pipeline that crawls web content to build semantic knowledge graphs and exposes them via MCP and FastAPI.

**Source credibility:** The project has 0 stars, but the high level of technical detail indicates professional engineering rather than a basic tutorial.

**Recency:** Very current; it explicitly incorporates modern AI patterns like MCP (Model Context Protocol).

**Source:** [butifugo/mt_agency_knowledge_graph/CLAUDE.md](https://github.com/butifugo/mt_agency_knowledge_graph/blob/f0a5d919d4a326f185512f11becd54079d9e34c6/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# mt_agency_knowledge_graph

Montana State Government **Knowledge Network**. Crawls 37+ state-agency websites (HTML, PDF,
DOCX), builds per-agency **knowledge graphs** with semantic relationships, derives **navigation
graphs**, and renders interactive D3 visualizations and a unified dashboard. The graph engine
in `src/network/` exposes a **graph-enhanced RAG retriever**, surfaced two ways over a single
shared retrieval core (`src/chat_api/retrieval.get_retriever`):

- **MCP server** (`src/mcp_server/`) — Python / FastMCP over **stdio**, so AI clients (Claude
  Desktop, etc.) can query agency knowledge directly. Not a network service; launched per-client.
- **Chat API** (`src/chat_api/`) — a FastAPI service (`/chat`, `/health`) that does retrieval +
  LLM synthesis, fronted by an embeddable browser widget in `web/` (`widget.js`).

## Pipeline mental model

```
agency websites (agencies.md)
        │  crawl + extract           src/phase1_crawl  (HTML/PDF/DOCX extractors)
        ▼
knowledge/{agency}/*.md  (markdown + frontmatter; generated, gitignored)
        │  build graph              src/phase2_knowledge  +  src/network/3_build_network.py
        ▼
data/graphs/knowledge/*.pkl  ·
```

</details>
