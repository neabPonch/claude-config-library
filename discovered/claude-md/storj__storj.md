---
name: storj__storj
source: https://github.com/storj/storj/blob/289df6ed095196358a6d7b404d15b9d5c54f43f3/CLAUDE.md
repo: storj/storj
kind: claude-md
stars: 3259
last_pushed: 2026-06-12T15:22:44Z
license: agpl-3.0
score: 9
domains: [backend, distributed-systems, go]
tags: [architecture, workflows, monolith]
curated: 2026-06-15
curated_by: config-scout
---

# storj/storj — claude-md

**Why it's worth keeping:** It includes concrete expansion workflows (adding services/schemas) and explains complex structural patterns like the 'Peer' architecture and monkit instrumentation idioms.

**Summary:** Provides deep architectural context, detailed subsystem hierarchies, and specific code patterns essential for navigating a large Go monolith.

**Source credibility:** High; Storj is a major decentralized storage project with significant star count and active maintenance.

**Recency:** Highly current, as evidenced by recent commit activity and modern Go development standards.

**Source:** [storj/storj/CLAUDE.md](https://github.com/storj/storj/blob/289df6ed095196358a6d7b404d15b9d5c54f43f3/CLAUDE.md) · 3259★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Storj Development Guide for Claude

## Overview

Storj is a decentralized cloud storage network where data is encrypted, split into pieces using erasure coding, and distributed across thousands of storage nodes worldwide. This repository contains the core components that power the network.

### Key Architectural Concepts

**Data Flow**: Files → Encryption → Erasure Coding (80 pieces, 29 needed to recover) → Distributed Storage Nodes → Metadata stored in Satellite

**Core Components**:
- **Satellite**: Centralized coordinator managing metadata, node selection, payments, and network health
- **Storage Nodes**: Distributed edge nodes storing encrypted file pieces
- **Uplink**: Client library for uploading/downloading data (separate repository)

## Build/Test/Lint Commands

- Build: `go build ./...` or `go build ./cmd/[component]`
- Test All: `make test`
- Single Test: `go test -v ./package/path -run TestName`
- Lint: `make llint`
- Lint only one package: `make llint LINT_TARGET=./<directory>`
- Format imports: `gci write --section Standard --section Default --section 'Prefix(storj.io/)' <file>`

### Running Unit Tests

By default run unit tests using Spanner.

## Code Style Guidelin
```

</details>
