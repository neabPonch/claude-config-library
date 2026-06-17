---
name: the-yash-rajput__AgentCrafter
source: https://github.com/the-yash-rajput/AgentCrafter/blob/fae3da74a7679a922bbae89a67ba580a3780ba5f/Claude.md
repo: the-yash-rajput/AgentCrafter
kind: claude-md
stars: 0
last_pushed: 2026-04-27T08:48:12Z
license: unknown
score: 9
domains: [backend-api, web-frontend, agents-ai, fullstack]
tags: [django, react, langgraph, architecture-mapping, schema-definitions]
curated: 2026-06-16
curated_by: config-scout
---

# the-yash-rajput/AgentCrafter — claude-md

**Why it's worth keeping:** The file provides critical 'tribal knowledge' like the distinction between two ORM layers, explicit database connection/pooling details, and comprehensive schema definitions that prevent hallucinated data structures.

**Summary:** A highly detailed technical blueprint for a full-stack AI orchestration platform covering Django backend and React frontend.

**Source credibility:** Low social proof (0 stars), but high technical density indicates a legitimate, well-architected project.

**Recency:** Very current; uses modern versions of LangGraph, Django, and React.

**Source:** [the-yash-rajput/AgentCrafter/Claude.md](https://github.com/the-yash-rajput/AgentCrafter/blob/fae3da74a7679a922bbae89a67ba580a3780ba5f/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AgentCrafter — Claude Reference

Full-stack visual AI workflow builder. Users design LangGraph agent graphs through a drag-and-drop UI; all configuration is stored in PostgreSQL and executed at runtime via LangGraph with PostgreSQL checkpointing.

---

## Repo Layout

```
AgentCrafter/
├── backend_django/          # Django REST API + LangGraph runtime
├── frontend/                # React + Vite + ReactFlow UI
├── docker-compose.yml       # postgres + backend + frontend
├── .vscode/launch.json      # debugpy attach config (port 5678)
└── CLAUDE.md                # this file
```

---

## Key Concepts

| Concept | Description |
|---------|-------------|
| **Agent** | Top-level workflow entity. Has `state_schema`, `entry_node`, `exit_nodes`. Status: `draft / active / archived`. |
| **AgentVersion** | Immutable snapshot of an agent's graph (nodes + edges + state_schema). Versions are forked, not edited in-place. |
| **Node** | A single operation in the graph. Has `type` (functional / llm_call / communication), `subtype`, and `config` (JSONB). |
| **Edge** | Connection between nodes. Either `direct` (unconditional) or `conditional` (routed by `condition_config`). |
| **Run** | One exec
```

</details>
