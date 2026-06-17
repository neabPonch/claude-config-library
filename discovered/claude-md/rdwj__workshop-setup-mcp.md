---
name: rdwj__workshop-setup-mcp
source: https://github.com/rdwj/workshop-setup-mcp/blob/15d6352731fa061e3c27339cc9abfd787462decb/CLAUDE.md
repo: rdwj/workshop-setup-mcp
kind: claude-md
stars: 0
last_pushed: 2026-06-12T20:37:42Z
license: unknown
score: 9
domains: [agents-ai, infrastructure-devops, security, backend-api]
tags: [mcp, openshift, k8s, python-agent, orchestration]
curated: 2026-06-16
curated_by: config-scout
---

# rdwj/workshop-setup-mcp — claude-md

**Why it's worth keeping:** The 'Lessons Learned' section captures critical platform-specific gotchas that prevent runtime errors, while the 'Agent Development Patterns' provides actionable code templates for extending functionality.

**Summary:** Provides comprehensive architectural context, deployment orchestration stages, and specific coding patterns for a complex MCP ecosystem on OpenShift.

**Source credibility:** Though the repo has 0 stars, the highly technical depth and specific versioning (v0.7.0) suggest high-quality professional engineering documentation.

**Recency:** Very current; includes specific nuances regarding the Model Context Protocol (MCP) ecosystem.

**Source:** [rdwj/workshop-setup-mcp/CLAUDE.md](https://github.com/rdwj/workshop-setup-mcp/blob/15d6352731fa061e3c27339cc9abfd787462decb/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Project Is

A hands-on workshop for deploying the MCP Ecosystem on Red Hat OpenShift AI. The repo contains:

- **Workshop modules** (`deploy/workshop/`) — step-by-step guides for deploying the MCP Gateway, MCP servers, identity/auth, and an agent
- **Platform base** (`deploy/base/`) — Kustomize overlay for cluster prerequisites (RHOAI, NFD, Authorino)
- **Demo stack** (`demo/`) — three components that form the end-to-end demo:
  - `demo/agent/` — Python/fipsagents AI agent with MCP tool integration
  - `demo/gateway/` — Go HTTP gateway (auth, file upload, routing)
  - `demo/ui/` — Go chat UI with streaming support
The agent itself is minimal (`demo/agent/src/agent.py` is ~30 lines). Most complexity lives in the authentication flow, the workshop deployment stages, and the framework (vendored, do not edit).

## Build and Test Commands

Agent commands (run from `demo/agent/`):

```bash
make install                         # Create .venv, install deps
make run-local                       # Start HTTP server on port 8080
make test                            #
```

</details>
