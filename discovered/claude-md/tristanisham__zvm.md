---
name: tristanisham__zvm
source: https://github.com/tristanisham/zvm/blob/f59f5452fd8af3cae9a2c29dabfe546ec9282075/CLAUDE.md
repo: tristanisham/zvm
kind: claude-md
stars: 1005
last_pushed: 2026-06-09T18:49:21Z
license: mit
score: 9
domains: [cli-tools, systems-programming, golang]
tags: [go, cli, architecture-mapping]
curated: 2026-06-15
curated_by: config-scout
---

# tristanisham/zvm — claude-md

**Why it's worth keeping:** The 'Architecture' section is top-tier; it explains how data structures initialize and where the most complex business logic resides. It also includes critical build tags and error-handling conventions that prevent AI from deviating from the project style.

**Summary:** This file provides excellent architectural mapping of a Go CLI tool, linking core logic flows to specific files and explaining platform-specific abstractions.

**Source credibility:** High; a popular tool (1k stars) with very recent maintenance activity.

**Recency:** Current; utilizes modern Go patterns like errors.Join() and contemporary CLI libraries.

**Source:** [tristanisham/zvm/CLAUDE.md](https://github.com/tristanisham/zvm/blob/f59f5452fd8af3cae9a2c29dabfe546ec9282075/CLAUDE.md) · 1005★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ZVM (Zig Version Manager) is a CLI tool written in Go for installing and managing multiple Zig compiler versions. It also supports installing ZLS (Zig Language Server). Built with `urfave/cli/v3`.

## Build & Test Commands

```bash
go build -v .                    # Build the binary
go test -v ./...                 # Run all tests
go test -v ./cli/ -run TestName  # Run a single test
go vet ./...                     # Static analysis
go fmt ./...                     # Format code
```

Build without self-upgrade capability (for package manager distributions):
```bash
go build -tags noAutoUpgrades .
```

## Architecture

**Entry point:** `main.go` — defines the CLI app with `urfave/cli/v3`. A `Before` hook initializes a global `ZVM` instance that all command handlers share.

**Core type:** `cli.ZVM` (in `cli/config.go`) holds `baseDir` (default `~/.zvm`) and `Settings`. Initialized via `Initialize()` which creates the directory structure and loads `~/.zvm/settings.json`.

**Key flows:**
- **Install** (`cli/install.go`): fetches version map → downloa
```

</details>
