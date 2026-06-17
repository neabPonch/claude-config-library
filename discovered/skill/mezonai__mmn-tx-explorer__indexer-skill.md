---
name: mezonai__mmn-tx-explorer__indexer-skill
source: https://github.com/mezonai/mmn-tx-explorer/blob/d92607fbb93d0b9e5baa70199b38f78e747d4cf9/.opencode/indexer-skill.md
repo: mezonai/mmn-tx-explorer
kind: skill
stars: 5
last_pushed: 2026-05-19T07:45:23Z
license: unknown
score: 8
domains: [backend, blockchain, cli-tools]
tags: [go, indexer, infrastructure]
curated: 2026-06-16
curated_by: config-scout
---

# mezonai/mmn-tx-explorer — skill

**Why it's worth keeping:** It includes high-value details like specific test execution patterns, directory-to-logic mapping, and architectural guardrails (e.g., reorg handling) that prevent AI hallucination of the project structure.

**Summary:** This skill file provides comprehensive structural and procedural context for a Go-based blockchain indexer service.

**Source credibility:** Based on a specialized blockchain infrastructure repository.

**Recency:** Highly current, utilizing modern Go 1.24 standards.

**Source:** [mezonai/mmn-tx-explorer/.opencode/indexer-skill.md](https://github.com/mezonai/mmn-tx-explorer/blob/d92607fbb93d0b9e5baa70199b38f78e747d4cf9/.opencode/indexer-skill.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Indexer Skill

## Overview
Blockchain indexer service written in Go. Syncs data from blockchain to PostgreSQL.

## Tech Stack
- Go 1.24 with Cobra CLI
- PostgreSQL (3 DBs: orchestrator, staging, main)
- Kafka for events
- Prometheus for metrics
- golangci-lint for linting

## Directory Structure
```
indexer/
├── cmd/           # CLI commands (Cobra-based)
├── api/           # HTTP API layer
├── internal/      # Core logic
│   ├── orchestrator/  # Block sync orchestration
│   ├── worker/       # Block processing
│   ├── rpc/          # RPC client
│   ├── storage/      # PostgreSQL storage
│   ├── handlers/     # HTTP handlers
│   ├── publisher/    # Kafka publisher
│   └── ...
├── configs/      # Configuration files
└── tools/        # Migration scripts
```

## Commands
```bash
cd indexer
docker-compose up -d postgres
go build -o main -tags=production

# Database migrations
./main migrate-postgres

# Run services
./main orchestrator   # Block indexer
./main api            # HTTP API server

# Other commands
./main sync_blocks
./main validate
./main validate_and_fix

# Test
go test ./... -v                              # All tests
go test ./internal/orchestrator -v            # Sin
```

</details>
