---
name: go-eagle__eagle
source: https://github.com/go-eagle/eagle/blob/b1301b093ebe53e2e12040e1c83f3a65e5b1ab4a/CLAUDE.md
repo: go-eagle/eagle
kind: claude-md
stars: 2424
last_pushed: 2026-04-22T22:46:29Z
license: mit
score: 8
domains: [backend-api, microservices, go]
tags: [architecture-mapping, cli-tools, dependency-injection]
curated: 2026-06-15
curated_by: config-scout
---

# go-eagle/eagle — claude-md

**Why it's worth keeping:** It explicitly maps the layered directory structure to business logic roles and provides critical documentation for a framework-specific CLI tool used for scaffolding.

**Summary:** Provides comprehensive development workflows including custom CLI commands, architectural layers, and dependency injection patterns.

**Source credibility:** Highly credible source with 2.4k stars and recent maintenance activity.

**Recency:** Current; specifically mentions Go 1.22+ support.

**Source:** [go-eagle/eagle/CLAUDE.md](https://github.com/go-eagle/eagle/blob/b1301b093ebe53e2e12040e1c83f3a65e5b1ab4a/CLAUDE.md) · 2424★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Eagle is a Go microservice framework suitable for rapid business development. It can quickly build API services or Web sites with support for HTTP and gRPC protocols.

## Essential Commands

### Development
```bash
# Run the main application
make run

# Build the binary (with version info)
make build

# Run tests
make test

# Run a single test
go test -v -run TestFunctionName ./path/to/package

# Run tests with coverage
make cover

# View test coverage in browser
make view-cover
```

### Code Quality
```bash
# Run linter (uses golangci-lint)
make lint

# Format code
make fmt

# Run vet
make vet
```

### Code Generation
```bash
# Generate Swagger documentation
make docs
# Access docs at: http://localhost:8080/swagger/index.html

# Generate mock files
make mockgen
```

### Other
```bash
# Clean build artifacts
make clean

# Build Docker image
make docker

# Generate CA certificates
make ca

# Generate call graph visualization
make graph
```

### Eagle CLI Tool
The project provides a CLI tool for code generation:
```bash
# Install the CLI
go install
```

</details>
