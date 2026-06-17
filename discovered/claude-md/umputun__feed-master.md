---
name: umputun__feed-master
source: https://github.com/umputun/feed-master/blob/a4226be8a0377cf23f2020cc936998278e327533/CLAUDE.md
repo: umputun/feed-master
kind: claude-md
stars: 141
last_pushed: 2026-03-19T09:02:34Z
license: mit
score: 9
domains: [backend, go, devops, cli-tools]
tags: [go, troubleshooting, production-context, deployment]
curated: 2026-06-15
curated_by: config-scout
---

# umputun/feed-master — claude-md

**Why it's worth keeping:** It includes 'Important Testing Notes' regarding hardcoded date logic in the code—a classic AI failure point—and detailed troubleshooting for yt-dlp/cookie edge cases.

**Summary:** A high-signal guide that maps architecture to directory structure and provides critical operational context for complex tool interactions.

**Source credibility:** High; comes from a well-maintained Go repository with significant star count.

**Recency:** Current; includes modern Go practices and specific deployment details relevant to today's workflows.

**Source:** [umputun/feed-master/CLAUDE.md](https://github.com/umputun/feed-master/blob/a4226be8a0377cf23f2020cc936998278e327533/CLAUDE.md) · 141★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build, Test, Lint Commands
```bash
# Run tests
go test -race -v ./...                            # Run all tests from root
go test -race -v ./app/...                        # Run app tests
go test -race -v ./app/proc                       # Test specific package
go test -race -v ./app/proc -run TestStore       # Run specific test

# Lint code
golangci-lint run ./...                           # Lint entire codebase from root
golangci-lint run ./app/...                       # Lint app directory

# Build application
cd app && go build -o feed-master                 # Build binary
docker build -t feed-master .                      # Build Docker image

# Format and normalize
gofmt -s -w $(find . -type f -name "*.go" -not -path "./vendor/*")
goimports -w $(find . -type f -name "*.go" -not -path "./vendor/*")
```

## High-Level Architecture

Feed Master is a Go service that aggregates RSS feeds and YouTube content into unified feeds:

- **app/main.go**: Entry point with CLI flags, initializes Processor and Server
- **app/proc**: Core feed processing logic
  - `Processo
```

</details>
