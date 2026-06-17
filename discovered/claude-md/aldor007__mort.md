---
name: aldor007__mort
source: https://github.com/aldor007/mort/blob/9cf57d34d282f9e37e8d9fac3d45b28d8c83984a/CLAUDE.md
repo: aldor007/mort
kind: claude-md
stars: 521
last_pushed: 2025-12-19T10:48:51Z
license: mit
score: 9
domains: [backend, image-processing, go]
tags: [architecture-heavy, pattern-focused, technical-nuance]
curated: 2026-06-15
curated_by: config-scout
---

# aldor007/mort — claude-md

**Why it's worth keeping:** It includes 'Common Development Patterns' to guide AI expansion and 'Important Implementation Details' that explain the reasoning behind complex logic rather than just the syntax.

**Summary:** A high-context guide that details architectural flows, specific build commands, and technical nuances like 'thundering herd' mitigation.

**Source credibility:** Highly credible; a specialized Go tool with significant GitHub popularity (521 stars).

**Recency:** Current; provides specific environment variable instructions relevant to modern CGO/libvips builds.

**Source:** [aldor007/mort/CLAUDE.md](https://github.com/aldor007/mort/blob/9cf57d34d282f9e37e8d9fac3d45b28d8c83984a/CLAUDE.md) · 521★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Mort is an S3-compatible image processing server written in Go. It transforms images on-the-fly using URL-based parameters (presets or query strings) and supports multiple storage backends (S3, local, HTTP, Azure, Google Cloud, etc.). The server handles request collapsing, rate limiting, caching, S3 GLACIER object restoration, and includes an S3-compatible API for listing and uploading files.

**New Feature:** Automatic S3 GLACIER/DEEP_ARCHIVE object restore - see [docs/GLACIER_RESTORE.md](docs/GLACIER_RESTORE.md)

## Build & Development Commands

### Running Tests
```bash
# Run unit tests with race detection and formatting
make unit

# Run unit tests with benchmarks
make unit-bench

# Run integration tests (requires npm dependencies)
make integrations

# Run all tests
make tests

# Run tests in docker
make docker-tests

# Generate coverage report
make coverage
```

### Running Single Tests
```bash
# Run specific test with race detection
go test -race -run TestName ./pkg/path/to/package

# Run tests in a single package
go test -race ./pkg/cache/.
```

</details>
