---
name: eduardolmedeiros__nomadfly
source: https://github.com/eduardolmedeiros/nomadfly/blob/62ff5cfbc46c913759721bb2ed811766f3270954/CLAUDE.md
repo: eduardolmedeiros/nomadfly
kind: claude-md
stars: 2
last_pushed: 2026-04-07T18:25:45Z
license: unknown
score: 8
domains: [cli-tools, agents-ai, backend]
tags: [go, mcp, architecture, tooling]
curated: 2026-06-15
curated_by: config-scout
---

# eduardolmedeiros/nomadfly — claude-md

**Why it's worth keeping:** The 'Key Conventions' section provides a clear step-by-step pattern for adding new tools, which is essential for maintaining consistency in agentic projects.

**Summary:** A highly detailed architectural guide that maps specific directories to their responsibilities and provides explicit workflows for extending the toolset.

**Source credibility:** Recent development (2 months ago) of a specialized infrastructure tool.

**Recency:** Very current; includes specific patterns for MCP and AI-native tool registration.

**Source:** [eduardolmedeiros/nomadfly/CLAUDE.md](https://github.com/eduardolmedeiros/nomadfly/blob/62ff5cfbc46c913759721bb2ed811766f3270954/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance for Claude Code when working in this repository.

## Project Overview

`nomadfly` is a Go CLI tool that wraps HashiCorp Nomad's HTTP API with an AI-powered interface. It supports any OpenAI-compatible LLM provider (Ollama, OpenAI, Gemini, Anthropic) and exposes five interaction modes: `prompt`, `chat`, `tui`, `web`, and `serve` (MCP server).

## Build & Run

```bash
make build                              # Compile to bin/nomadfly
make test                               # Run tests
make tidy                               # go mod tidy
make lint                               # golangci-lint run
./bin/nomadfly prompt "your question"   # Quick test
```

## Architecture

- `main.go` — entry point, delegates to `cmd/`
- `cmd/` — Cobra CLI commands (`serve`, `prompt`, `chat`, `tui`, `web`)
- `internal/config/` — Viper config loader (YAML + env vars)
- `internal/llm/` — OpenAI-compatible LLM client (`client.go`) and agentic tool-calling loop (`loop.go`)
- `internal/nomad/` — HTTP client for Nomad API (cluster, jobs, nodes, allocs, deployments, variables)
  - `types.go` — all API response structs (shared across all files in the package)
- `internal/
```

</details>
