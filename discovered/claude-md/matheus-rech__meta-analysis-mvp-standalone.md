---
name: matheus-rech__meta-analysis-mvp-standalone
source: https://github.com/matheus-rech/meta-analysis-mvp-standalone/blob/74e2966b12b1a221e048aa37379967b60dd1b8dc/CLAUDE.md
repo: matheus-rech/meta-analysis-mvp-standalone
kind: claude-md
stars: 0
last_pushed: 2026-04-29T03:58:21Z
license: mit
score: 8
domains: [cli-tools, agents-ai, data-science]
tags: [mcp, typescript, r-stats, polyglot]
curated: 2026-06-15
curated_by: config-scout
---

# matheus-rech/meta-analysis-mvp-standalone — claude-md

**Why it's worth keeping:** Excellent documentation of inter-process communication (JSON serialization via Rscript) and detailed data flow patterns that prevent LLM guesswork during cross-language debugging.

**Summary:** Explains the polyglot architecture of an MCP server bridging TypeScript/Node.js and R statistical scripts. It details session management, tool capabilities, and runtime-to-runtime communication protocols.

**Source credibility:** Single developer repository with a highly specific, technical implementation.

**Recency:** Very recent; aligns with modern MCP development patterns.

**Source:** [matheus-rech/meta-analysis-mvp-standalone/CLAUDE.md](https://github.com/matheus-rech/meta-analysis-mvp-standalone/blob/74e2966b12b1a221e048aa37379967b60dd1b8dc/CLAUDE.md) · 0★

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
