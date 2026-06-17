---
name: w3slley__bookcover-api
source: https://github.com/w3slley/bookcover-api/blob/dcdc8b0606e63de6a69f4c02256b225a58ceba88/CLAUDE.md
repo: w3slley/bookcover-api
kind: claude-md
stars: 261
last_pushed: 2026-04-24T20:56:39Z
license: mit
score: 9
domains: [backend-api, go]
tags: [architecture-mapping, command-reference, testing-strategy]
curated: 2026-06-15
curated_by: config-scout
---

# w3slley/bookcover-api — claude-md

**Why it's worth keeping:** The inclusion of 'Design Decisions' and 'Application Flow' provides the AI with essential architectural constraints, while specific test commands help it perform accurate verification.

**Summary:** A high-density documentation file for a Go REST API that outlines component interactions, command sequences, and testing coverage.

**Source credibility:** Strong; a well-starred repository with recent commits indicating active maintenance.

**Recency:** Current; references modern Go versions (1.23) and standard container orchestration workflows.

**Source:** [w3slley/bookcover-api/CLAUDE.md](https://github.com/w3slley/bookcover-api/blob/dcdc8b0606e63de6a69f4c02256b225a58ceba88/CLAUDE.md) · 261★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A Go-based REST API that fetches book cover images from Goodreads. Supports searching by book title/author or ISBN-13. Uses memcached for caching and is deployed via Kubernetes with Helm charts.

## Common Commands

### Development
```bash
# Run the application locally
go run cmd/api/main.go

# Run tests
go test ./internal/handler/...

# Build the binary
go build -o bin/server ./cmd/api
```

### Docker
```bash
# Build and run with Docker Compose
docker compose up --build

# Build Docker image manually
docker build -t bookcover-api .
```

### Testing
```bash
# Run all tests (handler, scraper, service)
make test

# Run tests with verbose output
make test-verbose

# Run with coverage
make test-coverage

# Generate HTML coverage report
make test-coverage-html

# Run a specific test
go test -v ./internal/handler -run TestBookcoverSearch_CacheHit
```

## Architecture

### Project Structure
```
bookcover-api/
├── cmd/api/              # Application entry point
│   └── main.go
├── internal/             # Private application code
│   ├── cache/
```

</details>
