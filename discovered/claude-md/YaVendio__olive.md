---
name: YaVendio__olive
source: https://github.com/YaVendio/olive/blob/49859142b92aaefa318fcfc88d509c013621ec5e/CLAUDE.md
repo: YaVendio/olive
kind: claude-md
stars: 43
last_pushed: 2026-04-06T21:23:44Z
license: mit
score: 9
domains: [agents-ai, backend-api, cli-tools]
tags: [python, llm-tools, fastapi, architecture]
curated: 2026-06-14
curated_by: config-scout
---

# YaVendio/olive — claude-md

**Why it's worth keeping:** The file-mapping table provides an excellent mental model for code navigation, and the technical explanation of the 'Inject' pattern is highly specific for agent understanding.

**Summary:** Defines a framework for exposing Python functions as remote LLM tools via REST API, covering both server and client architectures.

**Source credibility:** Moderate popularity (43 stars) with recent maintenance activity from 2 months ago.

**Recency:** Very current, utilizing modern Python standards including 3.12+ and advanced type hinting.

**Source:** [YaVendio/olive/CLAUDE.md](https://github.com/YaVendio/olive/blob/49859142b92aaefa318fcfc88d509c013621ec5e/CLAUDE.md) · 43★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## What is Olive

Olive is a Python framework for exposing functions as remote LLM-callable tools via REST API. Decorate with `@olive_tool`, get a FastAPI server with JSON Schema generation, context injection, optional Temporal durable execution, and client SDKs for LangChain/LangGraph/ElevenLabs.

## Philosophy

- **One decorator, zero boilerplate**: `@olive_tool` registers the function, extracts schemas from type hints, and exposes it via REST. The original function is returned unmodified.
- **Server owns tools, agent consumes them**: Tools are non-deterministic (HTTP, DB, APIs). Deterministic logic stays in the agent.
- **No hidden tools**: Every `@olive_tool` is visible to the LLM. Don't filter tools from the LLM's view.
- **Temporal is optional**: Works without Temporal (direct execution). Add `olive[temporal]` for durable workflows.

## Architecture

### Two Packages in One Wheel

- **`olive/`** — Server-side: decorator, registry, router, schema generation, CLI, Temporal worker
- **`olive_client/`** — Client SDK: `OliveClient` for loading tools into LangChain/LangGraph/ElevenLabs

### Core Flow

```
@olive_tool decorator → ToolRegistry (global singleton) → FastAP
```

</details>
