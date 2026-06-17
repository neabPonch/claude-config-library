---
name: ddev__ddev
source: https://github.com/ddev/ddev/blob/1b5581b83734497b231491c05855f60fcf7fb6b3/CLAUDE.md
repo: ddev/ddev
kind: claude-md
stars: 3653
last_pushed: 2026-06-14T18:49:08Z
license: apache-2.0
score: 9
domains: [cli-tools, devops, go]
tags: [build-systems, git-workflow, coding-standards, testing]
curated: 2026-06-15
curated_by: config-scout
---

# ddev/ddev — claude-md

**Why it's worth keeping:** Includes 'gotcha' warnings about IDE diagnostics, provides exact shell commands for preserving markdown in commits via stdin, and defines strict branch/commit naming conventions to ensure consistency.

**Summary:** A high-fidelity guide that covers not just the codebase structure, but also specific build/test nuances, coding style constraints, and rigorous Git workflow procedures.

**Source credibility:** High-quality source from a popular (3.6k+ stars) and actively maintained open-source project.

**Recency:** Extremely current; updated within the last month.

**Source:** [ddev/ddev/CLAUDE.md](https://github.com/ddev/ddev/blob/1b5581b83734497b231491c05855f60fcf7fb6b3/CLAUDE.md) · 3653★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

DDEV is an open-source tool for running local web development environments for PHP and Node.js. It uses Docker containers to provide consistent, isolated development environments with minimal configuration.

For developer documentation, see:

- [Developer Documentation](https://docs.ddev.com/en/stable/developers/)
- [Building and Contributing](docs/content/developers/building-contributing.md)

## Key Development Commands

### Building

**IMPORTANT: Always use `make` to build the DDEV binary, never `go build` directly.**

```bash
make                    # Build for host OS/arch. Output: .gotmp/bin/<os>_<arch>/ddev
make linux_amd64        # Cross-compile for specific platform
```

### Testing

```bash
go test -v ./pkg/[package]                    # Test specific package
make testpkg TESTARGS="-run TestName"         # Run subset of package tests
make testcmd TESTARGS="-run TestName"         # Run command tests
make quickstart-test                          # Run Bats docs tests
```

**Testing Tips:**

- Use subset testing with regex patterns for fast
```

</details>
