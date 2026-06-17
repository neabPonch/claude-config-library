---
name: deviceinsight__kafkactl
source: https://github.com/deviceinsight/kafkactl/blob/782e3959689e7f989a4adda2b62e927d98298e43/CLAUDE.md
repo: deviceinsight/kafkactl
kind: claude-md
stars: 1059
last_pushed: 2026-05-13T05:05:39Z
license: apache-2.0
score: 9
domains: [cli-tools, backend, infrastructure]
tags: [go, kafka, testing-patterns, architecture]
curated: 2026-06-14
curated_by: config-scout
---

# deviceinsight/kafkactl — claude-md

**Why it's worth keeping:** It explicitly defines test naming conventions/requirements and explains the specific Command Pattern used to route logic, which prevents AI hallucination during refactoring.

**Summary:** A high-quality project guide for a Go CLI tool that covers builds, complex integration testing with Docker, and internal architectural patterns.

**Source credibility:** High-quality open source project with significant stars and recent activity.

**Recency:** Very current; uses modern Go tool directives and up-to-date development workflows.

**Source:** [deviceinsight/kafkactl/CLAUDE.md](https://github.com/deviceinsight/kafkactl/blob/782e3959689e7f989a4adda2b62e927d98298e43/CLAUDE.md) · 1059★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - kafkactl Project Guide

## Project Overview

kafkactl is a command-line interface for Apache Kafka written in Go. It supports topic/consumer-group/ACL/broker/user management, message producing/consuming with Avro/Protobuf/JSON schema support, Kubernetes-proxied execution, and an external plugin system for OAuth token providers.

- **Module**: `github.com/deviceinsight/kafkactl/v5`
- **Go version**: 1.24.12
- **Kafka client**: IBM/sarama
- **CLI framework**: spf13/cobra + spf13/viper
- **License**: Apache 2.0

## Build & Run Commands

```bash
# Build the binary
make build

# Run all checks (fmt, lint, cve-check, test, build, docs)
make all

# Format code
make fmt                    # runs gofmt + goimports

# Lint (golangci-lint via Go tool directive)
make lint                   # runs: go tool golangci-lint run

# Unit tests only (skips integration tests)
make test                   # runs: go tool gotestsum --format testname --hide-summary=skipped -- -v -short ./...

# Integration tests (requires Docker)
make integration_test       # starts docker-compose cluster, runs tests, tears down

# CVE check
make cve-check              # runs: go tool govulncheck ./...

# Cle
```

</details>
