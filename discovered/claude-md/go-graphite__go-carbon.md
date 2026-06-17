---
name: go-graphite__go-carbon
source: https://github.com/go-graphite/go-carbon/blob/546c17b36ffc0b0d9d1e083b993de37dd447790f/CLAUDE.md
repo: go-graphite/go-carbon
kind: claude-md
stars: 827
last_pushed: 2026-06-08T10:03:37Z
license: mit
score: 9
domains: [backend, systems-programming, observability]
tags: [architecture, data-flow, golang, devops]
curated: 2026-06-15
curated_by: config-scout
---

# go-graphite/go-carbon — claude-md

**Why it's worth keeping:** The 'Architecture' section uses text-based data flow diagrams and a 'Common Patterns' section that defines specific developer behaviors (like lifecycle management and configuration types) crucial for maintaining consistency.

**Summary:** Extremely detailed guide that maps out the complete architectural pipeline from ingestion to persistence. It provides clear command instructions for testing, linting, and building within a vendored environment.

**Source credibility:** High; a well-established, actively maintained Go project with significant GitHub traction.

**Recency:** Current; explicitly mentions Claude Code and contemporary Go development practices like race detection and vendoring.

**Source:** [go-graphite/go-carbon/CLAUDE.md](https://github.com/go-graphite/go-carbon/blob/546c17b36ffc0b0d9d1e083b993de37dd447790f/CLAUDE.md) · 827★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

<!-- Generated: 2026-04-13 | Updated: 2026-04-13 -->

## What This Is

go-carbon is a high-performance Golang implementation of Graphite's carbon-cache daemon. It receives metrics via multiple protocols (TCP, UDP, Pickle, HTTP, Kafka, PubSub), buffers them in a sharded in-memory cache, and persists them to Whisper (.wsp) files. Also serves a read API (carbonserver) compatible with graphite-web and carbonapi.

## Build & Test Commands

```bash
make                    # Build the go-carbon binary
make test               # Run tests, vet, and race detection (all three)
go test ./...           # Run tests only (faster iteration)
go test -race ./...     # Run tests with race detector
go vet ./...            # Run vet only
go test -run TestName ./package/  # Run a single test
make image              # Build Docker image (requires Linux binary)
```

Dependencies use vendoring (`-mod=vendor` is set via GOFLAGS in the Makefile). Run `go mod tidy && go mod vendor` when updating dependencies.

## Linting

CI uses golangci-lint v2. Config is in `.golangci.yml`. Enabled linters:
```

</details>
