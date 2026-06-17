---
name: jaskirat-gill__InsightRAG
source: https://github.com/jaskirat-gill/InsightRAG/blob/5bbe51f976ea9e52b5992d685c7a0194ec5091dd/skill.md
repo: jaskirat-gill/InsightRAG
kind: skill
stars: 12
last_pushed: 2026-04-20T07:10:09Z
license: unknown
score: 8
domains: [agents-ai, search-rag]
tags: [mcp, rag, search-optimization, agent-guidance]
curated: 2026-06-14
curated_by: config-scout
---

# jaskirat-gill/InsightRAG — skill

**Why it's worth keeping:** It includes crucial search heuristics like 'short keyword first' and threshold adjustment logic. The 'Common Workflows' section is excellent for teaching agents how to navigate from discovery to specific searches.

**Summary:** A high-quality MCP skill reference that provides strategic instructions for an agent to interact with a RAG-based knowledge base.

**Source credibility:** Low (academic project), but the documentation structure reflects professional-grade agent instructions.

**Recency:** Recent; updated within the last 2 months and uses modern MCP patterns.

**Source:** [jaskirat-gill/InsightRAG/skill.md](https://github.com/jaskirat-gill/InsightRAG/blob/5bbe51f976ea9e52b5992d685c7a0194ec5091dd/skill.md) · 12★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# InsightRAG MCP Skill Reference

This document is a practical reference for both:

- LLMs deciding how to use the InsightRAG MCP tools effectively
- Human developers integrating with the InsightRAG service over MCP or raw HTTP

## Overview

InsightRAG exposes a knowledge base search server via the **Model Context Protocol (MCP)**. The server runs on port `8002` using HTTP transport (FastMCP framework). It provides hybrid vector + keyword search over document collections stored in Qdrant.

For LLM tool use, prefer the tool-calling guidance in this document. For direct service integrations, the authentication and transport details below also apply.

## Authentication

Direct HTTP requests require a bearer token issued by the sync-service auth system:

```
Authorization: Bearer <jwt_access_token>
```

- Tokens are JWTs signed with HS256, issued via the sync-service `/api/v1/auth/login` endpoint.
- The token's `sub` claim identifies the user; KB access is scoped per-user.
- Admin users can access all knowledge bases. Regular users see only owned or shared KBs.
- STDIO transport (local dev only) skips authentication.

If you are using these capabilities through an MCP host that already
```

</details>
