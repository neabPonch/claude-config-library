---
name: jerrelblankenship__jb-kibana-mcp
source: https://github.com/jerrelblankenship/jb-kibana-mcp/blob/a9c1f31d19d4530d824c81ec6b5e7d117b779722/CLAUDE.md
repo: jerrelblankenship/jb-kibana-mcp
kind: claude-md
stars: 2
last_pushed: 2026-03-06T22:36:24Z
license: unknown
score: 9
domains: [agents-ai, cli-tools, backend-api]
tags: [mcp, typescript, node, kibana]
curated: 2026-06-16
curated_by: config-scout
---

# jerrelblankenship/jb-kibana-mcp — claude-md

**Why it's worth keeping:** The 'Adding New Capabilities' workflow and specific logging instructions (using stderr for stdio) are highly transferable, expert-level technical constraints that prevent runtime errors.

**Summary:** Provides a deep architectural mental model of an MCP server, mapping out transport layers and the Kibana integration hierarchy. It serves as an excellent guide for how data flows from a protocol request to an external API.

**Source credibility:** Specialized tool with high-quality documentation structure and recent activity.

**Recency:** Very current; aligns perfectly with modern MCP and TypeScript development standards.

**Source:** [jerrelblankenship/jb-kibana-mcp/CLAUDE.md](https://github.com/jerrelblankenship/jb-kibana-mcp/blob/a9c1f31d19d4530d824c81ec6b5e7d117b779722/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

MCP (Model Context Protocol) server enabling AI assistants to interact with Kibana dashboards, visualizations, and Elasticsearch data. Wraps the Kibana REST API and exposes it via the MCP protocol over two transports: stdio (local) and HTTP/SSE (containerized).

## Development Commands

```bash
npm install                    # Install dependencies
npm run build                  # Compile TypeScript to dist/
npm run dev                    # Run stdio server via tsx
npm run dev:http               # Run HTTP server via tsx
npm run start:http             # Run HTTP server (production, from dist/)
npm run watch                  # TypeScript watch mode

# Testing (vitest)
npm test                       # Run all tests
npm run test:watch             # Watch mode
npm run test:coverage          # Coverage report
```

## Architecture

```
AI Assistant → MCP Protocol → MCP Server (this project) → Kibana REST API → Elasticsearch
```

**Two transport entry points share one core server:**
- `src/index.ts` — Stdio transport (local/Claude Desktop). Reads env var
```

</details>
