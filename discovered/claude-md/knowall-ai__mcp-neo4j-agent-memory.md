---
name: knowall-ai__mcp-neo4j-agent-memory
source: https://github.com/knowall-ai/mcp-neo4j-agent-memory/blob/d48e5e937756cfc83bf7fffc887f71defb026e7a/CLAUDE.md
repo: knowall-ai/mcp-neo4j-agent-memory
kind: claude-md
stars: 69
last_pushed: 2025-10-27T21:33:21Z
license: mit
score: 9
domains: [ai-agents, backend-api, cli-tools]
tags: [mcp, typescript, neo4j, pattern-driven]
curated: 2026-06-16
curated_by: config-scout
---

# knowall-ai/mcp-neo4j-agent-memory — claude-md

**Why it's worth keeping:** The 'Tool Implementation Pattern' section is a perfect example of how to instruct an AI to maintain code consistency through exact, repeatable steps.

**Summary:** Defines a three-layer architecture and provides high-density implementation patterns for extending the server.

**Source credibility:** A respected niche repository within the emerging MCP ecosystem.

**Recency:** Highly current, reflecting modern TypeScript patterns and MCP standards.

**Source:** [knowall-ai/mcp-neo4j-agent-memory/CLAUDE.md](https://github.com/knowall-ai/mcp-neo4j-agent-memory/blob/d48e5e937756cfc83bf7fffc887f71defb026e7a/CLAUDE.md) · 69★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an MCP (Model Context Protocol) server that bridges Neo4j graph database with Claude Desktop. It provides both basic Neo4j operations and specialized memory-focused tools optimized for AI agents and conversational AI.

## Key Architecture

The codebase follows a three-layer architecture:

1. **Entry Layer** (`src/index.ts`): Handles environment configuration and server lifecycle
2. **Server Layer** (`src/server.ts`): Implements MCP protocol with 10 specialized tools
3. **Client Layer** (`src/neo4j-client.ts`): Abstracts Neo4j driver operations

### Critical Design Decisions

- **Entity-Based Memory System**: The `remember`/`recall`/`connect_memories` tools promote storing separate nodes for each entity rather than complex properties
- **Type Guards**: Every tool has a corresponding `isXArgs()` function for runtime validation
- **Session Management**: Neo4j sessions are created per query and properly closed to prevent connection leaks
- **Integer Conversion**: Neo4j's Integer type is automatically converted to JavaScript numbers

## Develo
```

</details>
