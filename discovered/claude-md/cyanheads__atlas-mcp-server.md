---
name: cyanheads__atlas-mcp-server
source: https://github.com/cyanheads/atlas-mcp-server/blob/5a0bfdc08f9d0d106e69432bcaa606cc414340f1/CLAUDE.md
repo: cyanheads/atlas-mcp-server
kind: claude-md
stars: 477
last_pushed: 2025-07-22T05:17:41Z
license: apache-2.0
score: 8
domains: [agents-ai, backend-api, database, cli-tools]
tags: [mcp, neo4j, typescript, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# cyanheads/atlas-mcp-server — claude-md

**Why it's worth keeping:** The use of visual hierarchy trees for data relationships and specific architectural layering helps an agent navigate complex service dependencies; it also explicitly links configuration to Zod validation patterns.

**Summary:** Provides a structural blueprint for an MCP server using Neo4j, detailing the three-tier architecture from transport to data layers.

**Source credibility:** Strong; high star count (477) suggests a well-regarded tool in the MCP ecosystem.

**Recency:** Very current, focusing on the modern Model Context Protocol standard.

**Source:** [cyanheads/atlas-mcp-server/CLAUDE.md](https://github.com/cyanheads/atlas-mcp-server/blob/5a0bfdc08f9d0d106e69432bcaa606cc414340f1/CLAUDE.md) · 477★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Essential Development Commands

### Build and Development

- `npm run build` - Build the TypeScript project and make executable
- `npm run dev` - Watch mode for TypeScript compilation
- `npm run rebuild` - Clean and rebuild project completely
- `npm run format` - Format code with Prettier

### Database Operations

- `npm run db:backup` - Create database backup with timestamped directory
- `npm run db:import <backup_path>` - Restore database from backup (destructive)
- `docker-compose up -d` - Start Neo4j database
- `docker-compose down` - Stop Neo4j database

### Running the Server

- `npm run start:stdio` - Run with stdio transport (default for MCP clients)
- `npm run start:http` - Run with HTTP transport on localhost:3010
- `npm run inspector` - Run MCP inspector for debugging

### Testing and Quality

- `npm run webui` - Open basic web UI for viewing data
- `npm run tree` - Generate project structure documentation

## Core Architecture

ATLAS is an MCP (Model Context Protocol) server with a three-tier Neo4j-backed architecture:

**Transport Layer** (`src/mcp/tr
```

</details>
