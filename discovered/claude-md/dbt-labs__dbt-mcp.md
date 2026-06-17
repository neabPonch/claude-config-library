---
name: dbt-labs__dbt-mcp
source: https://github.com/dbt-labs/dbt-mcp/blob/6622aa4965581bc977d46ed5cdbd662901d45525/CLAUDE.md
repo: dbt-labs/dbt-mcp
kind: claude-md
stars: 577
last_pushed: 2026-06-16T13:18:19Z
license: apache-2.0
score: 9
domains: [agents-ai, cli-tools, backend]
tags: [mcp, python, architectural-patterns]
curated: 2026-06-16
curated_by: config-scout
---

# dbt-labs/dbt-mcp — claude-md

**Why it's worth keeping:** The 'Tool Architecture' section is excellent; it explains the required multi-step registration flow to prevent an AI from creating orphaned or inconsistent code. It also defines specialized metadata patterns for interactive UI apps.

**Summary:** Provides a deep architectural map of how MCP tools are registered and categorized within the system. It includes specific patterns for extending functionality via decorators and enums.

**Source credibility:** High; maintained by dbt Labs, a reputable organization in the data engineering space.

**Recency:** Very current; utilizes the modern Model Context Protocol (MCP) and up-to-date Python development practices.

**Source:** [dbt-labs/dbt-mcp/CLAUDE.md](https://github.com/dbt-labs/dbt-mcp/blob/6622aa4965581bc977d46ed5cdbd662901d45525/CLAUDE.md) · 577★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

dbt-mcp is an MCP (Model Context Protocol) server that exposes dbt functionality as tools to AI assistants. Built on `FastMCP` from the `mcp` SDK.

## Key Paths

- Entry point: `src/dbt_mcp/main.py`
- Server: `src/dbt_mcp/mcp/server.py` (`DbtMCP` class, `create_dbt_mcp()`)
- Tool infra: `src/dbt_mcp/tools/` (definitions, registration, injection, toolsets, tool_names)
- Tool categories: `discovery/`, `semantic_layer/`, `dbt_cli/`, `dbt_codegen/`, `dbt_admin/`, `lsp/`, `mcp_server_metadata/`
- Prompts (tool descriptions): `src/dbt_mcp/prompts/`
- Config: `src/dbt_mcp/config/`
- Tests: `tests/unit/`, `tests/integration/`

## Tool Architecture

Tools follow a consistent pattern:
1. `@dbt_mcp_tool` decorator defines the tool with metadata
2. `ToolName` enum in `tools/tool_names.py` — every tool needs an entry
3. Toolset mapping in `tools/toolsets.py` — maps tools to categories
4. Context injection via `adapt_context()` — tools receive typed context objects, but MCP only sees user-facing params
5. `register_tools()` in `tools/register.py` — precedence-based enablement (individual > toolset > default)

### MCP Apps (tools with interactive UI)

Tools can h
```

</details>
