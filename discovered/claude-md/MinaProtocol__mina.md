---
name: MinaProtocol__mina
source: https://github.com/MinaProtocol/mina/blob/26afa1f0130bbfa78d34a7c0b2c39df5b4d98f98/CLAUDE.md
repo: MinaProtocol/mina
kind: claude-md
stars: 2119
last_pushed: 2026-06-15T04:46:20Z
license: apache-2.0
score: 9
domains: [blockchain, cli-tools, backend-systems]
tags: [ocaml, monorepo, build-system, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# MinaProtocol/mina — claude-md

**Why it's worth keeping:** Includes 'Gotchas' like ulimit requirements and memory needs to prevent build failures; uses descriptive directory mapping so the AI understands the purpose of files rather than just their names.

**Summary:** A comprehensive guide that provides semantic context for a complex OCaml monorepo, covering build profiles, architectural layers, and system constraints.

**Source credibility:** High-profile blockchain protocol with active maintenance and significant community trust.

**Recency:** Very recent, reflecting modern high-complexity development workflows.

**Source:** [MinaProtocol/mina/CLAUDE.md](https://github.com/MinaProtocol/mina/blob/26afa1f0130bbfa78d34a7c0b2c39df5b4d98f98/CLAUDE.md) · 2119★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview
Mina Protocol is a lightweight blockchain that maintains constant size by using recursive zk-SNARKs. The codebase is primarily written in OCaml (4.14.2) with additional components in Go (libp2p helper) and Rust (cryptographic implementations via proof-systems submodule).

## Build Commands

### Core Build Commands
- `make build` - Build the Mina daemon and core executables (requires 10GB+ RAM)
- `make build-archive` - Build the archive node
- `make build-rosetta` - Build Rosetta API components
- `make libp2p_helper` - Build the Go libp2p helper (required for networking)
- `make build-intgtest` - Build integration test tools
- `make build-mainnet-sigs` - Build mainnet signature variants
- `make build-devnet-sigs` - Build devnet signature variants
- `make build-daemon-utils` - Build daemon utilities
- `make build-archive-utils` - Build archive node and related utilities
- `make build-test-utils` - Build test utilities
- `make build-replayer` - Build the replayer tool
- `make build-logproc` - Build log processor

### Quick Development Commands
- `dun
```

</details>
