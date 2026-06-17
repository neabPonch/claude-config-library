---
name: uber__kraken
source: https://github.com/uber/kraken/blob/f43117fdd57513f4c9454742c4e90383988bb043/CLAUDE.md
repo: uber/kraken
kind: claude-md
stars: 6699
last_pushed: 2026-06-12T15:37:44Z
license: apache-2.0
score: 9
domains: [distributed-systems, backend, infrastructure, go]
tags: [architectural-context, negative-constraints, operational-manual]
curated: 2026-06-15
curated_by: config-scout
---

# uber/kraken — claude-md

**Why it's worth keeping:** It utilizes 'negative constraints' (the 'Don't Do This' section) to prevent common AI mistakes and provides high-value debugging/profiling instructions.

**Summary:** A comprehensive guide that combines architectural context, specific build/test commands, and strict coding standards for a complex distributed system.

**Source credibility:** Extremely high; comes from a significant, active Uber open-source project.

**Recency:** Very recent; mentions Go 1.24 and has current maintenance patterns.

**Source:** [uber/kraken/CLAUDE.md](https://github.com/uber/kraken/blob/f43117fdd57513f4c9454742c4e90383988bb043/CLAUDE.md) · 6699★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Kraken Development Guide for Claude

## Project Overview

Kraken is a P2P-powered Docker registry designed for scalability and availability in hybrid cloud environments. It distributes Docker images using a BitTorrent-inspired protocol with a tracker-coordinated peer network. Built in Go, it has been in production at Uber since 2018, distributing over 1 million blobs per day.

**Key technologies**: Go 1.24+, Docker, Containerd, P2P networking, pluggable storage backends (S3, GCS, ECR, HDFS)

## Quick Start

### Build & Test
```bash
# Install dependencies
make vendor

# Build all binaries (uses Docker for cross-compilation on macOS)
make bins

# Build Docker images
make images

# Run unit tests
make unit-test

# Run integration tests (Python-based)
make integration

# Start local development cluster (requires Docker-for-Mac)
make devcluster
```

### Git Hooks
Install pre-commit hooks that run `golangci-lint` automatically:
```bash
make install-hooks
```

## Architecture Overview

Kraken consists of five main components forming a distributed system:

- **Agent** - Runs on every host, implements Docker registry API, P2P client/server
- **Origin** - Dedicated seeders, stores blobs ba
```

</details>
