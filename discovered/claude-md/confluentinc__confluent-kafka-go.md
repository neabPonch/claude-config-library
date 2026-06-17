---
name: confluentinc__confluent-kafka-go
source: https://github.com/confluentinc/confluent-kafka-go/blob/1994b47ccd54ef22c2fe75a2bac4b7aee6434912/CLAUDE.md
repo: confluentinc/confluent-kafka-go
kind: claude-md
stars: 5144
last_pushed: 2026-06-11T16:34:25Z
license: apache-2.0
score: 9
domains: [backend, distributed-systems, go]
tags: [cgo, kafka, integration-testing]
curated: 2026-06-15
curated_by: config-scout
---

# confluentinc/confluent-kafka-go — claude-md

**Why it's worth keeping:** Includes a high-value architectural mental model explaining the relationship between Go and C code; provides specific flags to manage Docker-based integration tests.

**Summary:** Provides essential context for building, testing (including complex integration scenarios), and understanding a CGo-heavy Go project.

**Source credibility:** High: Confluent is a major industry leader with a highly starred, actively maintained repository.

**Recency:** Current; reflects modern Go/Docker integration patterns suitable for Claude Code's agentic workflows.

**Source:** [confluentinc/confluent-kafka-go/CLAUDE.md](https://github.com/confluentinc/confluent-kafka-go/blob/1994b47ccd54ef22c2fe75a2bac4b7aee6434912/CLAUDE.md) · 5144★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

confluent-kafka-go is Confluent's Go client for Apache Kafka. It is a CGo wrapper around [librdkafka](https://github.com/confluentinc/librdkafka), a high-performance C library. The module path is `github.com/confluentinc/confluent-kafka-go/v2`.

## Build & Test Commands

### Building
```bash
# Default build (uses statically linked vendored librdkafka)
go build ./...

# Build with dynamically linked librdkafka (requires librdkafka installed via pkg-config)
go build -tags dynamic ./...
```

### Testing
```bash
# Run unit tests for the kafka package (no broker required)
go test ./kafka/...

# Run a single test
go test ./kafka/ -run TestLibraryVersion

# Run unit tests for schema registry
go test ./schemaregistry/...

# Integration tests live in a separate sub-module (kafka/integration/) so the
# testcontainers + testify deps don't bleed into the main kafka module's go.mod.
# Run them from within that module. Tests use docker-compose via testcontainers.
# Use these flags:
(cd kafka/integration && go test ./... -docker.needed)    # auto-starts Docker
```

</details>
