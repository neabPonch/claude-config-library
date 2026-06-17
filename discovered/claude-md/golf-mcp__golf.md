---
name: golf-mcp__golf
source: https://github.com/golf-mcp/golf/blob/df0004b8911d4bd8a896354e0f8732c3cdff0c64/CLAUDE.md
repo: golf-mcp/golf
kind: claude-md
stars: 830
last_pushed: 2026-05-08T14:44:01Z
license: apache-2.0
score: 9
domains: [agents-ai, mcp-server, python, cli-tools]
tags: [architecture, breaking-changes, workflow, component-system]
curated: 2026-06-15
curated_by: config-scout
---

# golf-mcp/golf — claude-md

**Why it's worth keeping:** The 'Breaking Changes' section prevents AI hallucinations of legacy APIs, while the Component System description provides essential spatial logic for file-based tool discovery.

**Summary:** Provides deep technical context including architectural patterns, component discovery rules, and explicit breaking change history to prevent regression errors.

**Source credibility:** Highly credible; high star count (830) and active maintenance history.

**Recency:** Very recent; includes specific version 0.2.x breaking changes.

**Source:** [golf-mcp/golf/CLAUDE.md](https://github.com/golf-mcp/golf/blob/df0004b8911d4bd8a896354e0f8732c3cdff0c64/CLAUDE.md) · 830★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Golf is a Python framework for building MCP (Model Context Protocol) servers with zero boilerplate. It automatically discovers, parses, and compiles Python files containing tools, resources, and prompts into a runnable FastMCP server.

## Breaking Changes in Golf 0.2.x

Golf 0.2.x introduces breaking changes to align with FastMCP 2.11.x:

- **Authentication System**: Complete rewrite using FastMCP's built-in auth providers (JWT, OAuth, Static tokens)
- **Legacy OAuth Removed**: Custom OAuth implementation replaced with standards-compliant FastMCP providers  
- **Configuration Changes**: `auth.py` configuration must be updated to use new auth configs (legacy `pre_build.py` supported)
- **Dependency Updates**: Requires FastMCP >=2.14.0
- **Removed Files**: Legacy `oauth.py` and `provider.py` files removed from auth module
- **Deprecated Functions**: `get_provider_token()` and OAuth-related helpers return None (legacy compatibility)

## Key Architecture

- **Component Discovery**: Golf automatically scans `tools/`, `resources/`, and `prompts/` direc
```

</details>
