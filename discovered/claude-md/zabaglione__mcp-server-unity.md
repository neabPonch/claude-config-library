---
name: zabaglione__mcp-server-unity
source: https://github.com/zabaglione/mcp-server-unity/blob/4765856b8cc43f6154995a7e39256cc513b64875/CLAUDE.md
repo: zabaglione/mcp-server-unity
kind: claude-md
stars: 10
last_pushed: 2025-07-12T04:28:25Z
license: mit
score: 8
domains: [game-dev, cli-tools, mcp-servers]
tags: [unity, typescript, architecture-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# zabaglione/mcp-server-unity — claude-md

**Why it's worth keeping:** The use of 'Critical Implementation Details' to highlight high-risk procedures (like .meta generation) is an elite technique for ensuring agentic reliability in sensitive environments.

**Summary:** Provides deep architectural context distinguishing between legacy file-based and modern bridge workflows. It includes critical operational side-effects required to prevent project breakage in Unity.

**Source credibility:** Reliable niche tool with 10 stars and highly specific documentation.

**Recency:** Modern; follows current best practices for providing structured context to AI agents.

**Source:** [zabaglione/mcp-server-unity/CLAUDE.md](https://github.com/zabaglione/mcp-server-unity/blob/4765856b8cc43f6154995a7e39256cc513b64875/CLAUDE.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

# Unity MCP Server - Project Knowledge Base

## Project Overview
Unity MCP Server is a Model Context Protocol (MCP) server that bridges AI assistants (like Claude) with Unity game development. It supports both legacy file-based operations (v2.x) and direct Unity Editor integration (v3.0.0 for Unity 6000+).

## Commands

### Build and Development
- `npm run build` - Compile TypeScript to JavaScript
- `npm run dev` - Watch mode for development
- `npm start` - Start MCP server (stdio mode for Claude Desktop)
- `npm run start:http` - Start HTTP API server (default port 3000)
- `npm run clean` - Clean build artifacts

### Optimized Mode
- `npm run start:optimized` - MCP server with streaming for large files
- `npm run start:http:optimized` - HTTP server with streaming

### Testing
- `npm test` - Run all tests
- `npm run test:unit` - Unit tests only
- `npm run test:integration` - Integration tests only  
- `npm run test:e2e` - End-to-end tests
- `npm run test:coverage` - Generate coverage report
- `npm run test:manual` - Interactive manual test runner
- `npm run test:perfo
```

</details>
