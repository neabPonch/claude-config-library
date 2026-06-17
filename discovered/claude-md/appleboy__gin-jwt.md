---
name: appleboy__gin-jwt
source: https://github.com/appleboy/gin-jwt/blob/5a7089dad5f0d957ff386bda78e35b3be6a21809/CLAUDE.md
repo: appleboy/gin-jwt
kind: claude-md
stars: 2968
last_pushed: 2026-06-13T07:47:01Z
license: mit
score: 9
domains: [backend-api, security]
tags: [golang, jwt, middleware, authentication]
curated: 2026-06-15
curated_by: config-scout
---

# appleboy/gin-jwt — claude-md

**Why it's worth keeping:** The 'Common Development Patterns' section is a gold standard; it provides explicit blueprints for adding new configuration options or storage backends to ensure consistency.

**Summary:** Provides deep architectural context, security constraints, and clear 'how-to' recipes for extending the library. It covers complex authentication flows and specific backend implementation patterns.

**Source credibility:** High-quality, widely used Go repository with nearly 3k stars and active maintenance.

**Recency:** Very current, referencing modern Go versions in the CI/CD section.

**Source:** [appleboy/gin-jwt/CLAUDE.md](https://github.com/appleboy/gin-jwt/blob/5a7089dad5f0d957ff386bda78e35b3be6a21809/CLAUDE.md) · 2968★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**gin-jwt** is a JWT authentication middleware for the Gin web framework. It provides RFC 6749 compliant OAuth 2.0 refresh tokens with pluggable storage backends (in-memory, Redis with client-side caching). The library supports direct token generation, multiple JWT providers via dynamic key functions, and comprehensive cookie/header token management.

## Development Commands

### Testing

```bash
# Run all tests with coverage
make test

# Run tests with race detection and coverage report
go test -v -race -coverprofile=coverage.out -covermode=atomic ./...

# Generate HTML coverage report
make coverage

# Run specific test
go test -v -run TestFunctionName ./...

# Run tests in a specific package
go test -v ./store/...
```

### Code Quality

```bash
# Format code (uses golangci-lint fmt with gofmt, gofumpt, goimports, golines)
make format

# Run linter
make lint

# Run go vet
make vet

# Clean test cache and coverage files
make clean
```

### Development Setup

```bash
# Install required development tools (golangci-lint)
make install-tools
```

###
```

</details>
