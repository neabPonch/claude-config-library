---
name: stacklok__toolhive
source: https://github.com/stacklok/toolhive/blob/c346ed763e410f3d217d7118a90bba76e8e6a9c2/CLAUDE.md
repo: stacklok/toolhive
kind: claude-md
stars: 1880
last_pushed: 2026-06-14T20:31:35Z
license: apache-2.0
score: 10
domains: [cli-tools, backend-go, devops, ai-agents]
tags: [modular-rules, meta-learning, agentic-workflows, high-fidelity]
curated: 2026-06-15
curated_by: config-scout
---

# stacklok/toolhive — claude-md

**Why it's worth keeping:** The 'Evolving Conventions' meta-instruction for capturing tribal knowledge is world-class, as are the specific 'Things That Will Bite You' anti-patterns that prevent environment mismatches.

**Summary:** A highly structured guide that leverages a modular rule system and specialized subagents for complex Go/Kubernetes development. It includes a unique mechanism for codifying new developer preferences into version-controlled rules.

**Source credibility:** High-quality source from a popular, actively maintained enterprise MCP project.

**Recency:** Highly current; integrates advanced Claude Code patterns like subagent invocation and skill usage.

**Source:** [stacklok/toolhive/CLAUDE.md](https://github.com/stacklok/toolhive/blob/c346ed763e410f3d217d7118a90bba76e8e6a9c2/CLAUDE.md) · 1880★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code when working with this repository.

## Project Overview

ToolHive is a lightweight, secure manager for MCP (Model Context Protocol: https://modelcontextprotocol.io) servers written in Go. It provides a CLI (`thv`), a Kubernetes operator (`thv-operator`), and a proxy runner (`thv-proxyrunner`) for container-based MCP server isolation.

## Build and Development Commands

```bash
task build            # Build the main binary
task install          # Install binary to GOPATH/bin
task lint             # Run linting
task lint-fix         # Fix linting issues (preferred over lint)
task test             # Unit tests (excluding e2e)
task test-e2e         # E2E tests (requires build first)
task test-all         # All tests (unit + e2e)
task test-coverage    # Tests with coverage analysis
task gen              # Generate mocks
task docs             # Generate CLI documentation
task build-image      # Build container image
task build-all-images # Build all container images
```

**IMPORTANT**: Always use `task` commands. Never run `go test`, `go build`, or `golangci-lint` directly -- the Taskfile has correct flags, exclusions, and environme
```

</details>
