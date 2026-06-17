---
name: gornskew__skewed-emacs
source: https://github.com/gornskew/skewed-emacs/blob/fa9d56538c22f16ddf44abea34dc67d1120cdc85/CLAUDE.md
repo: gornskew/skewed-emacs
kind: claude-md
stars: 36
last_pushed: 2026-05-13T21:59:17Z
license: other
score: 9
domains: [dev-ops, lisp, emacs, docker, mcp-integration]
tags: [mcp, docker, lisp, emacs, environment-setup]
curated: 2026-06-15
curated_by: config-scout
---

# gornskew/skewed-emacs — claude-md

**Why it's worth keeping:** Provides explicit MCP function names/signatures to eliminate guesswork and includes 'Verification Commands' so the agent can self-diagnose environmental health before executing tasks.

**Summary:** Detailed instructions for managing a complex Dockerized Emacs and Common Lisp environment via MCP services. It provides the agent with exact tool signatures to interact with remote development containers.

**Source credibility:** High; reflects a sophisticated, custom-built dev environment with active maintenance.

**Recency:** Extremely current; built specifically around modern MCP (Model Context Protocol) workflows.

**Source:** [gornskew/skewed-emacs/CLAUDE.md](https://github.com/gornskew/skewed-emacs/blob/fa9d56538c22f16ddf44abea34dc67d1120cdc85/CLAUDE.md) · 36★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Skewed Emacs + Gendl Docker Development Environment

This file provides guidance to Claude Code (claude.ai/code) when working with the integrated Skewed Emacs and Gendl development environment.

## Overview

This setup provides a complete Lisp development environment with:
- **Skewed Emacs Container**: Custom Emacs configuration with MCP integration
- **Gendl Container**: 3D CAD/modeling system with Common Lisp REPL and MCP integration
- **Network Integration**: Containers communicate via Docker network for SLIME connections
- **MCP Services**: Both containers expose services via Model Context Protocol for external tool integration

## MCP Integration

The containers are now wrapped as MCP (Model Context Protocol) services, providing seamless integration with Claude Code and other MCP-enabled tools.

### Available MCP Services

**Emacs Lisp Evaluation Service:**
- **Service Name**: `mcp__skewed-emacs__skewed-emacs__lisp_eval`
- **Purpose**: Evaluate Emacs Lisp code remotely
- **Usage**: `mcp__skewed-emacs__skewed-emacs__lisp_eval(code="(+ 1 2 3)")`

**Gendl Common Lisp Services (included with skewed-emacs):**
- `mcp__gendl_ccl__gendl_ccl__lisp_eval` — Gendl on Clozure CL (port 90
```

</details>
