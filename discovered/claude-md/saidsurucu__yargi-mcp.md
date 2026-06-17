---
name: saidsurucu__yargi-mcp
source: https://github.com/saidsurucu/yargi-mcp/blob/37681046796a44e1e5c9b893fcdc5330a8720184/CLAUDE.md
repo: saidsurucu/yargi-mcp
kind: claude-md
stars: 981
last_pushed: 2026-06-08T15:53:18Z
license: mit
score: 9
domains: [agents-ai, cli-tools, backend-api]
tags: [mcp, optimization-log, python, devops]
curated: 2026-06-15
curated_by: config-scout
---

# saidsurucu/yargi-mcp — claude-md

**Why it's worth keeping:** Uses 'Optimization Phases' to document intentional schema reductions/unifications, which prevents the AI from attempting to revert optimizations; includes highly detailed tool-specific debugging commands.

**Summary:** Provides exhaustive technical documentation for an MCP server, including specific command sets for development and testing.

**Source credibility:** High credibility with 981 stars and very recent maintenance.

**Recency:** Highly current; utilizes modern tooling like `uv` and the FastMCP protocol.

**Source:** [saidsurucu/yargi-mcp/CLAUDE.md](https://github.com/saidsurucu/yargi-mcp/blob/37681046796a44e1e5c9b893fcdc5330a8720184/CLAUDE.md) · 981★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a FastMCP server that provides programmatic access to Turkish legal databases through the Model Context Protocol (MCP). It integrates with 11 different Turkish legal institutions' databases including Yargıtay (Court of Cassation), Danıştay (Council of State), Constitutional Court, Competition Authority, Court of Accounts (Sayıştay), KVKK (Personal Data Protection Authority), BDDK (Banking Regulation and Supervision Agency), and others.

**🎯 HIGHLY OPTIMIZED**: This MCP server has been extensively optimized for token efficiency, achieving a **56.8% reduction** in MCP overhead (from 14,061 to 6,073 tokens) while maintaining full functionality.

**✅ PRODUCTION READY**: Fully deployed on Fly.io with OAuth 2.0 authentication, Bearer JWT token support, and Claude AI integration. Server successfully handles 21 Turkish legal database tools with cross-origin authentication.

## Key Commands

### Installation and Setup

#### PyPI Installation (Recommended)
```bash
# Install from PyPI (no Git required)
pip install yargi-mcp

# Run the MCP server (st
```

</details>
