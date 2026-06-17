---
name: renlabs-dev__torus-substrate
source: https://github.com/renlabs-dev/torus-substrate/blob/60f1069327f668d0fafd6ba3d3b666a4e24011b5/CLAUDE.md
repo: renlabs-dev/torus-substrate
kind: claude-md
stars: 24
last_pushed: 2026-05-06T09:48:21Z
license: mit-0
score: 9
domains: [blockchain, rust, systems-programming]
tags: [strict-rules, safety-critical, substrate]
curated: 2026-06-15
curated_by: config-scout
---

# renlabs-dev/torus-substrate — claude-md

**Why it's worth keeping:** Uses high-stakes imperative language ('MUST NEVER') to enforce critical patterns like zero-panic policies and saturating arithmetic; organizes rules by technical domain rather than just style.

**Summary:** Provides ultra-strict, safety-critical coding standards for Substrate blockchain development to prevent runtime panics and state corruption.

**Source credibility:** The highly specialized nature of the rules suggests a professional, security-focused development team despite the relatively low star count.

**Recency:** Very current; reflects modern Rust/Substrate best practices and sophisticated developer workflows.

**Source:** [renlabs-dev/torus-substrate/CLAUDE.md](https://github.com/renlabs-dev/torus-substrate/blob/60f1069327f668d0fafd6ba3d3b666a4e24011b5/CLAUDE.md) · 24★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides strict guidance to Claude Code when working with this Substrate blockchain repository. These rules are non-negotiable and must be followed exactly.

## Project Overview

Torus is a stake-driven peer-to-peer network built on Substrate. The blockchain manages agents (validators and miners), token emissions, staking, and governance. Code quality is critical - runtime panics will halt the entire chain.

## References

- @README.md - Project overview, quick start, network setup
- @CONTRIBUTING.md - Development setup (Nix), guidelines, testing
- @docs/pallet-structure.md - Architecture and API design
- @docs/xtask-manual.md - Development tooling guide
- @docs/linear-emission.md - Token distribution algorithm

## Core Pallets

- **`torus0`**: Agent registration, staking, burn mechanisms, fee management
- **`emission0`**: Token distribution with linear emission algorithm, weight control
- **`governance`**: Proposals, voting, treasury, roles (allocators, curators)
- **`permission0`**: Permission and access control

### Permission0 Pallet Structure

The `permission0` pallet manages delegated permissions and access control within the Torus network. Key componen
```

</details>
