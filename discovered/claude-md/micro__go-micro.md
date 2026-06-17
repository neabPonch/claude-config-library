---
name: micro__go-micro
source: https://github.com/micro/go-micro/blob/e4d2a41c32924c6cb3ba9cd09cb10ef6a34ffa94/CLAUDE.md
repo: micro/go-micro
kind: claude-md
stars: 22778
last_pushed: 2026-06-15T19:25:54Z
license: apache-2.0
score: 9
domains: [backend, distributed-systems, go, ai-agents]
tags: [architecture-mapping, build-instructions, roadmap-driven]
curated: 2026-06-15
curated_by: config-scout
---

# micro/go-micro — claude-md

**Why it's worth keeping:** The 'Current Focus' section provides essential guardrails for task prioritization, while the annotated project structure explains intent rather than just paths.

**Summary:** Provides high-density context including annotated directory maps, explicit build/test commands, and strategic mission priorities.

**Source credibility:** Very high; go-micro is a major established Go framework with significant community traction.

**Recency:** Extremely current; includes specific 2026 roadmap milestones and focuses on cutting-edge AI/MCP integration.

**Source:** [micro/go-micro/CLAUDE.md](https://github.com/micro/go-micro/blob/e4d2a41c32924c6cb3ba9cd09cb10ef6a34ffa94/CLAUDE.md) · 22778★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Go Micro Project Guide

## Project Overview

Go Micro is a framework for distributed systems development in Go. It provides pluggable abstractions for service discovery, RPC, pub/sub, config, auth, storage, and more.

The framework is evolving into an **AI-native platform** where every microservice is automatically accessible to AI agents via the Model Context Protocol (MCP).

## Build & Test

```bash
# Run all tests
make test

# Run tests for a specific package
go test ./gateway/mcp/...
go test ./ai/...
go test ./model/...

# Lint
make lint

# Format
make fmt

# Build CLI
go build -o micro ./cmd/micro

# Run locally with hot reload
micro run
```

## Project Structure

```
go-micro/
├── agent/          # Agent abstraction (intelligent service management)
├── ai/             # AI model providers (Anthropic, OpenAI, Gemini, etc.)
├── auth/           # Authentication (JWT, no-op)
├── broker/         # Message broker (NATS, RabbitMQ)
├── cache/          # Caching (Redis)
├── client/         # RPC client (gRPC)
├── cmd/micro/      # CLI tool (run, deploy, mcp, build, server)
├── codec/          # Message codecs (JSON, Proto)
├── config/         # Dynamic config (env, file,
```

</details>
