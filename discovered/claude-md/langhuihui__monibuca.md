---
name: langhuihui__monibuca
source: https://github.com/langhuihui/monibuca/blob/34997f87b0da40dc5ce3aef5ef3d1cc3882f5d70/CLAUDE.md
repo: langhuihui/monibuca
kind: claude-md
stars: 2385
last_pushed: 2026-04-28T15:00:57Z
license: agpl-3.0
score: 9
domains: [backend, streaming-media]
tags: [architecture-guide, go-language, plugin-system, asynchronous-tasks]
curated: 2026-06-15
curated_by: config-scout
---

# langhuihui/monibuca — claude-md

**Why it's worth keeping:** It explains high-leverage patterns like the Task/Job/Work hierarchy and cross-plugin communication strategies with concrete code examples. The inclusion of specific Go build tags is essential for navigating its multi-module capabilities.

**Summary:** Provides deep architectural context for a modular streaming framework, specifically detailing a complex asynchronous task management system.

**Source credibility:** Highly credible; a major, actively maintained open-source streaming project with significant community interest.

**Recency:** Very current; reflects modern development practices and active repository maintenance.

**Source:** [langhuihui/monibuca/CLAUDE.md](https://github.com/langhuihui/monibuca/blob/34997f87b0da40dc5ce3aef5ef3d1cc3882f5d70/CLAUDE.md) · 2385★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Monibuca is a high-performance streaming server framework written in Go. It's designed to be a modular, scalable platform for real-time audio/video streaming with support for multiple protocols including RTMP, RTSP, HLS, WebRTC, GB28181, and more.

## Development Commands

### Building and Running

**Basic Run (with SQLite):**
```bash
cd example/default
go run -tags sqlite main.go
```

**Build Tags:**
- `sqlite` - Enable SQLite database support
- `sqliteCGO` - Enable SQLite with CGO
- `mysql` - Enable MySQL database support  
- `postgres` - Enable PostgreSQL database support
- `duckdb` - Enable DuckDB database support
- `disable_rm` - Disable memory pool
- `fasthttp` - Use fasthttp instead of net/http
- `taskpanic` - Enable panics for testing

**Protocol Buffer Generation:**
```bash
# Generate all proto files
sh scripts/protoc.sh

# Generate specific plugin proto
sh scripts/protoc.sh plugin_name
```

**Release Building:**
```bash
# Uses goreleaser configuration
goreleaser build
```

**Testing:**
```bash
go test ./...
```

## Architecture Overview
```

</details>
