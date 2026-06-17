---
name: scalus3__scalus
source: https://github.com/scalus3/scalus/blob/38fa6a0f574e01b1cbe297c70578f69bd6e77368/Claude.md
repo: scalus3/scalus
kind: claude-md
stars: 102
last_pushed: 2026-06-12T20:23:06Z
license: apache-2.0
score: 9
domains: [blockchain, smart-contracts, compiler-engineering, scala]
tags: [sbt, multi-module, compilation-pipeline, scalafmt]
curated: 2026-06-14
curated_by: config-scout
---

# scalus3/scalus — claude-md

**Why it's worth keeping:** Includes highly useful mappings of sbt projects to module purposes and explicit instructions for handling incremental compilation stale states. The negative constraint against adding 'Co-authored by Claude Code' is a professional touch that prevents messy git histories.

**Summary:** A comprehensive guide mapping complex multi-module sbt projects to specific source locations and command use cases.

**Source credibility:** High; active maintenance (updated 0 months ago) and specialized domain expertise in Cardano/Scala.

**Recency:** Current; incorporates modern Scala 3 syntax and specific guidance for agentic workflows.

**Source:** [scalus3/scalus/Claude.md](https://github.com/scalus3/scalus/blob/38fa6a0f574e01b1cbe297c70578f69bd6e77368/Claude.md) · 102★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Guidelines for Scalus Project

## Project Overview

Scalus is a platform for developing decentralized applications (DApps) on Cardano.
It compiles a subset of Scala 3 to Scalus Intermediate Representation (SIR) and then
lowers to Untyped Plutus Core (UPLC), the language of Cardano smart contracts.

**For smart contract development:** Use `/contract` skill
**For smart contract testing:** Use `/contract-test` skill

## Commands

Prefer `sbtn` over `sbt`, when `sbtn` is aviable and not hangs. 

| Command          | Purpose                                              |
|------------------|------------------------------------------------------|
| `sbtn quick`     | Format, compile, jvm/testQuick (fast iteration)      |
| `sbtn testQuick` | Run only tests affected by recent changes            |
| `sbtn ci`        | Full CI: format check, all platforms, docs, mima     |
| `sbtn it`        | Integration tests (requires Docker)                  |

**Compilation:**

- `sbtn jvm/Test/compile` - all JVM projects with tests
- `sbtn scalusJVM/Test/compile` - scalus-core JVM with tests
- `sbtn scalusCardanoLedgerJVM/compile` - cardano-ledger JVM without tests
- `sbtn "clean; Test/c
```

</details>
