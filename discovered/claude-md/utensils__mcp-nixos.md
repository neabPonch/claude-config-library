---
name: utensils__mcp-nixos
source: https://github.com/utensils/mcp-nixos/blob/0ef99b6a5674e60ca315dc55a0f458673bb1e4fa/CLAUDE.md
repo: utensils/mcp-nixos
kind: claude-md
stars: 676
last_pushed: 2026-06-10T18:44:06Z
license: mit
score: 9
domains: [agents-ai, cli-tools, backend-api]
tags: [mcp, python, nixos, asyncio]
curated: 2026-06-16
curated_by: config-scout
---

# utensils/mcp-nixos — claude-md

**Why it's worth keeping:** The 'Never bypass linting' rule is a brilliant way to maintain code quality, and the explicit breakdown of async/blocking handling prevents subtle bugs during development.

**Summary:** Provides high-density technical context including detailed file mappings, environment-specific development workflows (Nix vs Python), and architectural constraints.

**Source credibility:** High; popular open-source project with 676 stars and very recent maintenance.

**Recency:** Current; uses modern FastMCP patterns and contemporary Python async practices.

**Source:** [utensils/mcp-nixos/CLAUDE.md](https://github.com/utensils/mcp-nixos/blob/0ef99b6a5674e60ca315dc55a0f458673bb1e4fa/CLAUDE.md) · 676★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

MCP-NixOS is a Model Context Protocol (MCP) server that provides accurate, real-time information about NixOS packages, configuration options, Home Manager, nix-darwin, and flakes. It prevents AI assistants from hallucinating about NixOS package names and configurations by querying official APIs and documentation.

## Project Structure & Module Organization

- `mcp_nixos/` - Contains the MCP server implementation.
  - `mcp_nixos/server.py` - MCP tools, tool routing, and main entry point.
  - `mcp_nixos/config.py` - Configuration constants (API URLs, auth, limits).
  - `mcp_nixos/caches.py` - Cache implementations (channels, nixvim, noogle, nix.dev).
  - `mcp_nixos/utils.py` - Shared utility functions (HTML parsing, formatting, file I/O).
  - `mcp_nixos/sources/` - Data source implementations (one module per source):
    - `base.py` - Channel helpers, Elasticsearch queries, browsing utilities.
    - `nixos.py` - NixOS packages/options search, info, stats.
    - `home_manager.py` - Home Manager options.
    - `darwin.py` - nix-darwin options.
    -
```

</details>
