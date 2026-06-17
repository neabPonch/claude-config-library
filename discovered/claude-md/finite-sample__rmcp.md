---
name: finite-sample__rmcp
source: https://github.com/finite-sample/rmcp/blob/389b6ef608a2ebc01b15f7dca3cd7fe71509e406/CLAUDE.md
repo: finite-sample/rmcp
kind: claude-md
stars: 201
last_pushed: 2025-12-28T05:22:01Z
license: mit
score: 9
domains: [cli-tools, data-science, backend-api]
tags: [hybrid-environment, step-by-step-workflow, testing-tiers]
curated: 2026-06-15
curated_by: config-scout
---

# finite-sample/rmcp — claude-md

**Why it's worth keeping:** The dual-path command structure (local UV vs. Docker) tells an AI agent exactly when to use fast tools versus when to use the full environment; it also includes a perfect procedural workflow for adding new features.

**Summary:** A high-quality guide featuring a 'hybrid development strategy' that distinguishes between lightweight Python tasks and heavy R/Docker integrations.

**Source credibility:** Strong; 201 stars and follows modern toolchain standards like 'uv'.

**Recency:** Current; uses modern Python tooling (uv, ruff) and specific MCP patterns.

**Source:** [finite-sample/rmcp/CLAUDE.md](https://github.com/finite-sample/rmcp/blob/389b6ef608a2ebc01b15f7dca3cd7fe71509e406/CLAUDE.md) · 201★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview
RMCP (R Model Context Protocol) is a statistical analysis server that bridges AI assistants with R statistical computing capabilities through the Model Context Protocol.

## Development Commands

### Setup & Running (Hybrid Approach)

**For Python-only development (cross-platform):**
```bash
uv sync --group dev              # Install minimal Python dependencies
uv run rmcp start                # Start server in stdio mode (no R tools)
uv run rmcp serve-http           # Start HTTP server with SSE

# Use configuration options
uv run rmcp --debug start        # Enable debug mode
uv run rmcp --config config.json start  # Use custom config file
RMCP_LOG_LEVEL=DEBUG uv run rmcp start  # Use environment variables
```

**For R integration development (Docker-based):**
```bash
docker build -f docker/Dockerfile --target development -t rmcp-dev .  # Build R + Python dev environment
docker run -v $(pwd):/workspace -it rmcp-dev bash
# Inside container:
cd /workspace && pip install -e .
rmcp start                        # Full R integration available
```

**For
```

</details>
