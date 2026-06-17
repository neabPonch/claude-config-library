---
name: kayac__go-katsubushi
source: https://github.com/kayac/go-katsubushi/blob/4380afea15b8b3700e4e6fe4f4f08cb20cb05919/CLAUDE.md
repo: kayac/go-katsubushi
kind: claude-md
stars: 196
last_pushed: 2026-06-12T13:27:23Z
license: mit
score: 8
domains: [backend, distributed-systems, go]
tags: [high-concurrency, snowflake, microservices]
curated: 2026-06-14
curated_by: config-scout
---

# kayac/go-katsubushi — claude-md

**Why it's worth keeping:** Contains critical low-level implementation constraints like specific slog usage patterns and time injection (nowFunc) to ensure test determinism.

**Summary:** Provides strict development guidelines for a high-concurrency Go service involving multi-protocol support and Redis coordination.

**Source credibility:** High; well-maintained, active open-source project with significant star count for a specialized utility.

**Recency:** Very current, utilizing modern Go standards such as the log/slog package.

**Source:** [kayac/go-katsubushi/CLAUDE.md](https://github.com/kayac/go-katsubushi/blob/4380afea15b8b3700e4e6fe4f4f08cb20cb05919/CLAUDE.md) · 196★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# go-katsubushi Development Notes

## Project Architecture

**Core Service**: Unique ID generation service using Snowflake-like algorithm
- **Multi-protocol support**: memcached-compatible, HTTP API, gRPC
- **Auto worker ID assignment**: Redis-based distributed worker management
- **Graceful shutdown**: Context-based lifecycle management across all protocols

**Key Components**:
- `app.go` - Main application logic and custom slog handler
- `generator.go` - Snowflake-like ID generation algorithm
- `memcache.go`, `http.go`, `grpc.go` - Protocol implementations
- `cmd/katsubushi/main.go` - CLI entry point

## Build & Deployment

### Build Tools
- `make all` - Generate gRPC code and build binary
- `make test` - Run tests with race detection
- `make packages` - Cross-platform builds with GoReleaser
- `make docker` - Multi-architecture Docker builds
- `aqua` for CLI tool management
- `buf` for Protocol Buffers generation

### Deployment Options
- Standalone execution (manual worker ID)
- Redis-coordinated auto worker ID assignment
- Docker/Kubernetes deployment
- Unix Domain Socket support

## Development Practices

### Code Patterns
- **Context management**: Graceful shutdown across all
```

</details>
