---
name: matheus-rech__lobby
source: https://github.com/matheus-rech/lobby/blob/01adcad29f9123971f2d7c3b0c33e489042dca26/CLAUDE.md
repo: matheus-rech/lobby
kind: claude-md
stars: 0
last_pushed: 2026-04-29T03:57:43Z
license: unknown
score: 8
domains: [cli-tools, data-science, backend]
tags: [typescript, r, mcp, statistical-computing]
curated: 2026-06-15
curated_by: config-scout
---

# matheus-rech/lobby — claude-md

**Why it's worth keeping:** Clearly documents cross-process communication patterns, explicit file system structures for session management, and specific tool definitions.

**Summary:** Explains how an MCP server orchestrates R statistical processes using TypeScript and JSON serialization.

**Source credibility:** Low social proof (0 stars), but the technical detail suggests a functional, niche implementation.

**Recency:** Highly current; leverages modern MCP (Model Context Protocol) standards.

**Source:** [matheus-rech/lobby/CLAUDE.md](https://github.com/matheus-rech/lobby/blob/01adcad29f9123971f2d7c3b0c33e489042dca26/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Meta-Analysis MVP (Minimum Viable Product) that implements a Model Context Protocol (MCP) server for conducting complete meta-analyses. The system integrates TypeScript/Node.js with R statistical computing to provide comprehensive meta-analysis capabilities.

## Architecture

### Core Components

1. **MCP Server** (TypeScript/Node.js)
   - Entry point: `src/index.ts`
   - Handles MCP protocol communication via stdio
   - Routes tool calls to appropriate handlers
   - Manages sessions through file-based storage

2. **R Statistical Engine**
   - Main dispatcher: `scripts/mcp_server.R` and `scripts/mcp_tools.R`
   - Tool implementations: Individual R scripts for each analysis function
   - Uses `metafor` and `meta` packages for statistical computations

3. **Session Management**
   - File-based storage in `sessions/` directory
   - Each session has its own directory with data/, results/, and processing/ subdirectories
   - No database required - uses JSON files for metadata

## Development Commands

```bash
# Install dependencies
npm insta
```

</details>
