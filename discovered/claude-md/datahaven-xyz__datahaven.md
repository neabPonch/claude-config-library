---
name: datahaven-xyz__datahaven
source: https://github.com/datahaven-xyz/datahaven/blob/edcb13dbbcd3c29489eaa2480a6f60ee4cb1f3ec/CLAUDE.md
repo: datahaven-xyz/datahaven
kind: claude-md
stars: 7946
last_pushed: 2026-04-17T12:27:11Z
license: gpl-3.0
score: 9
domains: [blockchain, rust, smart-contracts]
tags: [multilingual, workflow-driven, infrastructure]
curated: 2026-06-15
curated_by: config-scout
---

# datahaven-xyz/datahaven — claude-md

**Why it's worth keeping:** Includes proactive 'Common Pitfalls' and explicit code generation triggers to maintain type safety across components. Command grouping by sub-directory is highly effective for LLM tool use.

**Summary:** Defines a complex multi-stack blockchain environment involving Rust, TypeScript, and Solidity. It maps out the full development lifecycle from local setup to E2E testing.

**Source credibility:** High; significant star count (7.9k) and recent activity suggest a production-grade codebase.

**Recency:** Very current, specifically mentioning modern tools like Bun v1.2+.

**Source:** [datahaven-xyz/datahaven/CLAUDE.md](https://github.com/datahaven-xyz/datahaven/blob/edcb13dbbcd3c29489eaa2480a6f60ee4cb1f3ec/CLAUDE.md) · 7946★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

DataHaven is an EVM-compatible Substrate blockchain secured by EigenLayer. It bridges Ethereum and Substrate ecosystems through:
- EigenLayer AVS integration for security
- Snowbridge for cross-chain communication
- Frontier pallets for EVM compatibility
- External validators with rewards system

## Pre-requisites

- [Kurtosis](https://docs.kurtosis.com/install): For launching test networks
- [Bun](https://bun.sh/) v1.2+: TypeScript runtime and package manager
- [Docker](https://www.docker.com/): For container management
- [Foundry](https://getfoundry.sh/): For smart contract compilation/deployment
- [Helm](https://helm.sh/): Kubernetes package manager
- [Zig](https://ziglang.org/) (macOS only): For crossbuilding the node

## Critical Development Commands

### E2E Testing Environment (from `/test` directory)

```bash
# Setup
bun i                               # Install dependencies
bun cli                            # Interactive CLI for test environment

# Code Quality
bun fmt:fix                        # Fix TypeScript formatting (Biome)
bun t
```

</details>
