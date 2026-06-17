---
name: roadrunner-server__roadrunner
source: https://github.com/roadrunner-server/roadrunner/blob/e83e82dc4de3b4f172095e82a2b0f63194e9b802/CLAUDE.md
repo: roadrunner-server/roadrunner
kind: claude-md
stars: 8475
last_pushed: 2026-06-11T10:54:20Z
license: mit
score: 9
domains: [backend-infrastructure, cli-tools, go-development]
tags: [plugin-architecture, dependency-injection, process-manager]
curated: 2026-06-16
curated_by: config-scout
---

# roadrunner-server/roadrunner — claude-md

**Why it's worth keeping:** Includes a prescriptive 'Adding New Plugins' workflow and categorized lists of core components that enable precise code navigation. It also proactively lists module exclusions to prevent the LLM from suggesting incompatible dependencies.

**Summary:** Provides a highly structured overview of the plugin-based architecture, dependency injection mechanics, and specific command patterns for development.

**Source credibility:** High; highly starred project with very active maintenance.

**Recency:** Current; includes modern Go requirements and configuration standards.

**Source:** [roadrunner-server/roadrunner/CLAUDE.md](https://github.com/roadrunner-server/roadrunner/blob/e83e82dc4de3b4f172095e82a2b0f63194e9b802/CLAUDE.md) · 8475★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

RoadRunner is a high-performance PHP application server and process manager written in Go. It supports running as a service with extensive plugin functionality for HTTP/2/3, gRPC, queues (RabbitMQ, Kafka, SQS, NATS), KV stores, WebSockets, Temporal workflows, and more.

## Development Commands

### Build
```bash
make build
# Or manually:
CGO_ENABLED=0 go build -trimpath -ldflags "-s" -o rr cmd/rr/main.go
```

### Test
```bash
make test
# Or manually:
go test -v -race ./...
```

### Debug
```bash
make debug
# Uses delve to debug with sample config
```

### Run RoadRunner
```bash
./rr serve -c .rr.yaml
```

### Other Commands
```bash
./rr workers          # Show worker status
./rr workers -i       # Interactive worker information
./rr reset            # Reset workers
./rr jobs             # Jobs management commands
./rr stop             # Stop RoadRunner server
```

### Run Single Test
```bash
go test -v -race -run TestName ./path/to/package
```

## Architecture

### Plugin System

RoadRunner uses the **Endure** dependency injection container. All
```

</details>
