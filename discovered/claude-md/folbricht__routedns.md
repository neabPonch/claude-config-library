---
name: folbricht__routedns
source: https://github.com/folbricht/routedns/blob/0f133e150d5294be6dfaf9af8815b975414832db/CLAUDE.md
repo: folbricht/routedns
kind: claude-md
stars: 613
last_pushed: 2026-06-12T18:01:36Z
license: bsd-3-clause
score: 9
domains: [networking, cli-tools, backend]
tags: [go, dns, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# folbricht/routedns — claude-md

**Why it's worth keeping:** The 'Pipeline Flow' diagram and 'Key Patterns' section are exceptional for teaching an AI how to extend the system while maintaining architectural integrity via composition.

**Summary:** Provides a clear mental model of the DNS pipeline architecture and core interfaces alongside practical Go build/test instructions.

**Source credibility:** High-quality, well-maintained networking tool with over 600 stars and recent activity.

**Recency:** Highly relevant; provides the structural context required for high-level reasoning in modern agentic coding tools.

**Source:** [folbricht/routedns/CLAUDE.md](https://github.com/folbricht/routedns/blob/0f133e150d5294be6dfaf9af8815b975414832db/CLAUDE.md) · 613★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

RouteDNS is a composable DNS stub resolver, proxy and router written in Go. It builds processing pipelines from four component types (listeners, resolvers, groups/modifiers, routers) configured via TOML files.

## Build & Test Commands

```bash
# Build
go build -o cmd/routedns/ ./cmd/routedns

# Run all tests
go test ./...

# Run a single test
go test -run TestCacheLookupAndExpiry ./...

# Run tests in a specific package
go test ./dnssec/

# Run with race detector
go test -race ./...

# Run the binary
routedns config.toml
```

There is no Makefile or linter configuration. CI uses GitHub Actions: a build workflow runs `go build` and `go test -race ./...` on every PR and push to master, plus CodeQL analysis. Pushes to master trigger an automatic version bump and release.

## Architecture

### Core Abstraction

Every component in the pipeline implements the `Resolver` interface (`resolver.go`):

```go
type Resolver interface {
    Resolve(*dns.Msg, ClientInfo) (*dns.Msg, error)
    fmt.Stringer
}
```

This single interface is implemented by clients,
```

</details>
