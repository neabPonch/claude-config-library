---
name: celestiaorg__celestia-core
source: https://github.com/celestiaorg/celestia-core/blob/34f03e9ca116b29cdcbb3b831a786b26da4253c3/CLAUDE.md
repo: celestiaorg/celestia-core
kind: claude-md
stars: 552
last_pushed: 2026-06-12T16:16:00Z
license: apache-2.0
score: 9
domains: [blockchain, go, systems]
tags: [build-automation, architecture-guide, negative-constraints]
curated: 2026-06-14
curated_by: config-scout
---

# celestiaorg/celestia-core — claude-md

**Why it's worth keeping:** Uses effective negative constraints to prevent common mistakes and provides a high-density semantic map of the modular package structure.

**Summary:** Provides exhaustive build command documentation, package architecture mapping, and strict developer workflow rules.

**Source credibility:** High; comes from a major, actively maintained blockchain infrastructure project.

**Recency:** Very current; includes up-to-date branching strategies and modern Go toolchain instructions.

**Source:** [celestiaorg/celestia-core/CLAUDE.md](https://github.com/celestiaorg/celestia-core/blob/34f03e9ca116b29cdcbb3b831a786b26da4253c3/CLAUDE.md) · 552★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Celestia-core is a fork of CometBFT (formerly Tendermint) — a BFT consensus engine — with Celestia-specific modifications for data availability. The Go module path is `github.com/cometbft/cometbft`. It maintains minimal divergence from upstream CometBFT.

**Active branches:**
- `main`: Development for celestia-app

PRs should generally target `main` first, then backport to `v0.39.x-celestia` using the `backport-to-v0.39.x` label.

## Build Commands

```bash
make build                # Build binary to build/cometbft
make install              # Install to GOBIN
make test                 # Run all unit tests (go test -p 1 -tags deadlock)
make test_race            # Run tests with race detector
make test_cover           # Run tests with coverage
make test_integrations    # Full integration test suite (requires Docker)
make lint                 # Run golangci-lint
make format               # Run gofmt + goimports
make vulncheck            # Run govulncheck
make lint-typo            # Run codespell for typo checking
make proto-gen            # Generate
```

</details>
