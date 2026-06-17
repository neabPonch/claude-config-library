---
name: tky0065__go-starter-kit
source: https://github.com/tky0065/go-starter-kit/blob/080c1e0b4bff05c008b27bdb819e1ad17026d5fa/CLAUDE.md
repo: tky0065/go-starter-kit
kind: claude-md
stars: 2
last_pushed: 2026-03-25T18:27:53Z
license: unknown
score: 9
domains: [cli-tools, go]
tags: [scaffolding, automation, workflow-standardization]
curated: 2026-06-14
curated_by: config-scout
---

# tky0065/go-starter-kit — claude-md

**Why it's worth keeping:** The distinction between 'this repository' and 'generated structure' prevents AI context confusion. The explicit 'Documentation Update Process' provides an excellent template for maintaining project-wide consistency during development.

**Summary:** Provides comprehensive execution workflows and distinguishes between the CLI tool's source code and its generated project output. It enforces a strict documentation maintenance protocol.

**Source credibility:** Low star count, but the file demonstrates high-level engineering rigor through its structured workflows.

**Recency:** Current; uses modern Go command patterns and assumes contemporary toolchain availability.

**Source:** [tky0065/go-starter-kit/CLAUDE.md](https://github.com/tky0065/go-starter-kit/blob/080c1e0b4bff05c008b27bdb819e1ad17026d5fa/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is `go-starter-kit`, a Go CLI tool generator that scaffolds new Go projects. The tool is called `create-go-starter` and helps bootstrap Go project structures.

## Commands

### Build and Install
```bash
# Build the binary
go build -o create-go-starter ./cmd/create-go-starter

# Install the binary to GOBIN (typically ~/go/bin/)
go install ./cmd/create-go-starter

# Run directly without installing
go run ./cmd/create-go-starter <project-name>
```

### Testing
```bash
# Run all tests
go test ./...

# Run tests in a specific package
go test ./cmd/create-go-starter

# Run tests with verbose output
go test -v ./...

# Run a specific test function
go test -run TestColors ./cmd/create-go-starter

# Run tests with coverage report
go test -cover ./...

# Using Makefile targets
make test              # Run all tests
make test-short        # Quick unit tests (skip long-running tests)
make smoke-test        # Full E2E validation with runtime tests
make smoke-test-quick  # E2E validation without runtime (no Docker needed)
```

### Development
```bash
# Fo
```

</details>
