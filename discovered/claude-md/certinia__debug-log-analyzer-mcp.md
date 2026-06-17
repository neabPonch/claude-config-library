---
name: certinia__debug-log-analyzer-mcp
source: https://github.com/certinia/debug-log-analyzer-mcp/blob/e7d8f21c50c5d4088ead0cf326ee901c14359d60/CLAUDE.md
repo: certinia/debug-log-analyzer-mcp
kind: claude-md
stars: 15
last_pushed: 2026-05-18T16:56:40Z
license: bsd-3-clause
score: 8
domains: [mcp-servers, cli-tools, backend-logic]
tags: [typescript, mcp, salesforce, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# certinia/debug-log-analyzer-mcp — claude-md

**Why it's worth keeping:** It goes beyond file lists by explaining complex logic (like conditional tool registration) and the semantic shape of key data structures.

**Summary:** Provides a comprehensive architectural mental model including data structures and specific MCP tool behaviors.

**Source credibility:** A specialized niche project with recent maintenance activity.

**Recency:** Very current, updated within the last month.

**Source:** [certinia/debug-log-analyzer-mcp/CLAUDE.md](https://github.com/certinia/debug-log-analyzer-mcp/blob/e7d8f21c50c5d4088ead0cf326ee901c14359d60/CLAUDE.md) · 15★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the Apex Log MCP Server - a Model Context Protocol (MCP) server for Apex Log Analysis. It provides AI agents with tools to analyze Salesforce Apex debug logs for performance bottlenecks and optimization opportunities.

## Development Commands

```bash
# Install dependencies
pnpm install

# Build the TypeScript project
pnpm run build

# Development with watch mode
pnpm run dev

# Run the server standalone
pnpm start
```

## Architecture

### Core Components

- **src/index.ts**: Main MCP server implementation (`ApexLogServer` class)
  - Implements 4 MCP tools: `analyze_apex_log_performance`, `get_apex_log_summary`, `find_performance_bottlenecks`, `execute_anonymous`
  - Uses stdio transport for communication
  - Handles file validation, log parsing, analysis, and anonymous Apex execution

- **src/ApexLogParser.ts**: Complex log parsing engine (33k+ tokens)
  - Exports `parse()` function and `ApexLogParser` class
  - Handles Apex debug log format parsing into structured data
  - Tracks governor limits, performance metrics, and log issues

##
```

</details>
