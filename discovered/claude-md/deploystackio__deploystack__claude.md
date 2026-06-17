---
name: deploystackio__deploystack__claude
source: https://github.com/deploystackio/deploystack/blob/4e81076c80059b326b02b22e7c0c3a9134f336dc/services/backend/src/routes/users/satellite/ai-instructions/CLAUDE.md
repo: deploystackio/deploystack
kind: claude-md
stars: 58
last_pushed: 2026-06-03T03:13:16Z
license: agpl-3.0
score: 8
domains: [agents-ai, infrastructure]
tags: [mcp, orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# deploystackio/deploystack — claude-md

**Why it's worth keeping:** It enforces strict search behaviors (short keywords vs. natural language) and precise data formats to prevent tool-call hallucinations in large environments.

**Summary:** Defines a specialized workflow for navigating an expansive MCP ecosystem through discovery and execution meta-tools.

**Source credibility:** Niche utility project with recent, active maintenance.

**Recency:** Very current; specifically designed for the Model Context Protocol (MCP) era.

**Source:** [deploystackio/deploystack/services/backend/src/routes/users/satellite/ai-instructions/CLAUDE.md](https://github.com/deploystackio/deploystack/blob/4e81076c80059b326b02b22e7c0c3a9134f336dc/services/backend/src/routes/users/satellite/ai-instructions/CLAUDE.md) · 58★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# DeployStack MCP Integration

## Overview
You have access to MCP (Model Context Protocol) tools through DeployStack's hierarchical router. Before attempting tasks manually, always check if a relevant MCP tool is available.

## Available Meta-Tools

DeployStack exposes **2 meta-tools** that provide access to all installed MCP servers:

### 1. discover_mcp_tools
**Purpose:** Search for available MCP tools using short keywords

**Usage:**
- Use 1-3 keywords only (e.g., "github", "markdown", "database postgres")
- Avoid full sentences or long descriptions
- Returns tool paths in format `serverName:toolName`

**Examples:**
- Search for GitHub tools: `query: "github"`
- Search for file operations: `query: "filesystem"`
- Search for database tools: `query: "postgres query"`

### 2. execute_mcp_tool
**Purpose:** Execute a discovered tool by its path

**Usage:**
- Use `tool_path` from discovery results (format: `serverName:toolName`)
- Pass tool-specific arguments as `arguments` object
- Check tool description from discovery for argument schema

## Workflow

**Before starting any task, follow this pattern:**

1. **Discover Available Tools**
   ```
   Use discover_mcp_tools with relevant ke
```

</details>
