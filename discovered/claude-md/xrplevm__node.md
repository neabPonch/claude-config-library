---
name: xrplevm__node
source: https://github.com/xrplevm/node/blob/2d77d0981135a44b689175fb35fb22158cb773b1/CLAUDE.md
repo: xrplevm/node
kind: claude-md
stars: 1267
last_pushed: 2026-06-09T12:09:46Z
license: apache-2.0
score: 9
domains: [blockchain, security, go]
tags: [security-audit, invariants, cosmos-sdk]
curated: 2026-06-15
curated_by: config-scout
---

# xrplevm/node — claude-md

**Why it's worth keeping:** The 'key security invariants' section is exceptional; it provides the LLM with hard rules of correctness that are vital for high-stakes domain-specific work.

**Summary:** Provides project structure and a highly sophisticated workflow for conducting AI-driven security audits.

**Source credibility:** High; comes from an active, specialized blockchain infrastructure repository (XRPL EVM).

**Recency:** Very current; leverages advanced agentic orchestration patterns designed for modern AI tools.

**Source:** [xrplevm/node/CLAUDE.md](https://github.com/xrplevm/node/blob/2d77d0981135a44b689175fb35fb22158cb773b1/CLAUDE.md) · 1267★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

XRPL EVM Sidechain node (`exrpd`) — a Cosmos SDK-based blockchain node that runs an EVM-compatible sidechain for the XRP Ledger. Uses Proof-of-Authority consensus with authority-gated validator management.

## Build & Test

```bash
make build                # Build the exrpd binary
make test                 # Run unit tests
make lint                 # Run linter
go vet ./...              # Vet all packages
```

## Project Structure

```
cmd/exrpd/          # CLI entry point and node configuration
app/                # Cosmos SDK app wiring, ante handlers, upgrade handlers
app/ante/           # Transaction validation (routes EVM vs Cosmos txs)
x/poa/              # Proof-of-Authority module (validator add/remove)
proto/              # Protobuf definitions (gRPC API surface)
types/              # Core types (address prefixes, denominations)
testutil/           # Test helpers
tests/              # Integration tests
security/           # Security audit scope and threat model
```

## Security Audits

This repo is configured for monthly AI-assisted security audits. Before performing any security-related review, read:

1. **`.claude/security/SECURITY_SCOP
```

</details>
