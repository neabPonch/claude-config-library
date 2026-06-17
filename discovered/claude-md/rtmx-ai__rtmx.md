---
name: rtmx-ai__rtmx
source: https://github.com/rtmx-ai/rtmx/blob/cbbf501663ade2521ab2812f3c37a028914dc3f2/CLAUDE.md
repo: rtmx-ai/rtmx
kind: claude-md
stars: 25
last_pushed: 2026-06-08T10:34:14Z
license: apache-2.0
score: 9
domains: [cli-tools, go-backend, systems-programming]
tags: [cli, go, architectural-constraints, tdd, workflow-driven]
curated: 2026-06-15
curated_by: config-scout
---

# rtmx-ai/rtmx — claude-md

**Why it's worth keeping:** The use of custom slash commands (/tui-dev) to enforce persona/architecture boundaries and the inclusion of explicit dependency isolation rules are top-tier techniques.

**Summary:** This file provides highly structured domain-specific instructions, including specialized 'skills' for TUI and GUI development to maintain architectural integrity.

**Source credibility:** High; shows professional-grade engineering rigor through detailed parity, versioning, and CI instructions.

**Recency:** Very current; explicitly optimized for agentic workflows and modern CLI development.

**Source:** [rtmx-ai/rtmx/CLAUDE.md](https://github.com/rtmx-ai/rtmx/blob/cbbf501663ade2521ab2812f3c37a028914dc3f2/CLAUDE.md) · 25★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code when working with the RTMX Go CLI codebase.

## Overview

This is the Go implementation of the RTMX CLI, providing a single static binary for requirements traceability management. It is a port of the Python CLI (`rtmx-ai/rtmx`).

## Quick Commands

```bash
make build        # Build the binary
make test         # Run tests
make lint         # Run linter (golangci-lint v2 required)
make hooks        # Install pre-commit hooks
make dev          # Build with race detector
make build-all    # Build for all platforms
make parity       # Run parity tests against Python CLI
```

## Local CI Parity

**CRITICAL: Local pre-commit hooks must match remote CI checks.** Run `make hooks` after cloning to install `.githooks/pre-commit` which runs build, test, lint, and vet before each commit. This prevents pushing code that fails CI.

Install golangci-lint v2 if not present:
```bash
curl -sSfL https://raw.githubusercontent.com/golangci/golangci-lint/HEAD/install.sh | sh -s -- -b $(go env GOPATH)/bin
```

## Project Structure

```
rtmx/
├── cmd/rtmx/           # Main entry point
├── internal/
│   ├── cmd/            # CLI commands (Cobra)
│   ├
```

</details>
