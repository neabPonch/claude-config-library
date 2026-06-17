---
name: graphprotocol__graph-node
source: https://github.com/graphprotocol/graph-node/blob/07ae9302bcdac4f49ea7d511eae7ff683969cd94/CLAUDE.md
repo: graphprotocol/graph-node
kind: claude-md
stars: 3139
last_pushed: 2026-06-16T14:50:53Z
license: apache-2.0
score: 9
domains: [blockchain, rust, backend, infrastructure]
tags: [rust, testing-strategies, verification-patterns, strict-workflow]
curated: 2026-06-16
curated_by: config-scout
---

# graphprotocol/graph-node — claude-md

**Why it's worth keeping:** It includes 'Test Verification Requirements' to prevent the AI from assuming success when filters yield zero tests, and uses strong 'MANDATORY' directives for linting/formatting.

**Summary:** Provides highly specific command workflows for complex Rust/Cargo workspaces including detailed environment prerequisites and architecture mappings.

**Source credibility:** High; comes from a major production-grade blockchain indexing protocol with high star count and recent activity.

**Recency:** Very current, reflecting modern development workflows.

**Source:** [graphprotocol/graph-node/CLAUDE.md](https://github.com/graphprotocol/graph-node/blob/07ae9302bcdac4f49ea7d511eae7ff683969cd94/CLAUDE.md) · 3139★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Graph Node is a Rust-based decentralized blockchain indexing protocol that enables efficient querying of blockchain data through GraphQL. It's the core component of The Graph protocol, written as a Cargo workspace with multiple crates organized by functionality.

## Essential Development Commands

### Testing Workflow

⚠️ **Only run integration tests when explicitly requested or when changes require full system testing**

Use unit tests for regular development and only run integration tests when:

- Explicitly asked to do so
- Making changes to integration/end-to-end functionality
- Debugging issues that require full system testing
- Preparing releases or major changes

### Unit Tests

Unit tests are inlined with source code.

**Prerequisites:**

1. PostgreSQL running on localhost:5432 (with initialised `graph-test` database)
2. IPFS running on localhost:5001
3. PNPM
4. Foundry (for smart contract compilation)
5. Environment variable `THEGRAPH_STORE_POSTGRES_DIESEL_URL` set to `postgresql://graph:graph@127.0.0.1:5432/graph-test`

The environment
```

</details>
