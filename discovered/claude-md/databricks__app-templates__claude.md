---
name: databricks__app-templates__claude
source: https://github.com/databricks/app-templates/blob/113b615917b47617ccc44e53dd0b2715c52e1bf7/mcp-server-hello-world/Claude.md
repo: databricks/app-templates
kind: claude-md
stars: 155
last_pushed: 2026-06-15T07:20:58Z
license: other
score: 9
domains: [agents-ai, backend-api, cloud-infrastructure]
tags: [mcp, databricks, python, fastapi]
curated: 2026-06-15
curated_by: config-scout
---

# databricks/app-templates — claude-md

**Why it's worth keeping:** The 'Important Notes for AI Assistants' section is a masterclass in providing guardrails (like mandatory type hints/docstrings) to ensure the agent maintains codebase integrity and follows complex auth patterns.

**Summary:** A highly detailed guide for developing an MCP server on Databricks, covering architecture, authentication nuances, and deployment workflows.

**Source credibility:** High; sourced from an official Databricks template repository that is actively maintained.

**Recency:** Extremely current; focuses on the Model Context Protocol (MCP), which is a modern standard for AI tool-calling.

**Source:** [databricks/app-templates/mcp-server-hello-world/Claude.md](https://github.com/databricks/app-templates/blob/113b615917b47617ccc44e53dd0b2715c52e1bf7/mcp-server-hello-world/Claude.md) · 155★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude.md - MCP Server Hello World

This file provides context about this project for AI assistants like Claude.

## Project Overview

This is a **Model Context Protocol (MCP) server** template built with FastMCP and FastAPI, designed to run as a Databricks App. MCP enables AI assistants to discover and invoke tools/functions exposed by servers.

**Key Concepts:**
- **MCP Server**: Exposes tools via the Model Context Protocol over HTTP
- **Tools**: Python functions decorated with `@mcp_server.tool` that AI assistants can call
- **Databricks Apps**: The deployment platform where this server runs in production
- **Local Development**: Server runs on `localhost:8000` for testing before deployment

## Project Structure

```
server/              # Core MCP server code
├── app.py          # FastAPI + FastMCP setup, middleware
├── main.py         # Entry point (uvicorn runner)
├── tools.py        # MCP tool definitions (add new tools here)
└── utils.py        # Databricks auth helpers (workspace client factory)

scripts/            # Developer utilities
└── dev/
    ├── start_server.sh         # Start the MCP server locally
    ├── query_remote.sh         # Interactive remote deployment
```

</details>
