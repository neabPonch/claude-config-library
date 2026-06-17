---
name: ComeOnOliver__skillshub__skill
source: https://github.com/ComeOnOliver/skillshub/blob/db216d3a3d5eef365d1ff27ef240f644e918f05a/skills/trailofbits/skills/cosmos-vulnerability-scanner/SKILL.md
repo: ComeOnOliver/skillshub
kind: skill
stars: 52
last_pushed: 2026-05-25T04:16:34Z
license: mit
score: 9
domains: [blockchain, security, backend-go]
tags: [cosmos, security-audit, blockchain, determinism, golang]
curated: 2026-06-16
curated_by: config-scout
---

# ComeOnOliver/skillshub — skill

**Why it's worth keeping:** It provides specific shell command heuristics (grep patterns) for detecting subtle bugs and uses a highly professional 'Vulnerable vs Recommended' reporting structure.

**Summary:** A high-precision security auditing skill for Cosmos SDK and CosmWasm that targets consensus-critical vulnerabilities like non-determinism.

**Source credibility:** The content demonstrates deep domain expertise in blockchain security and protocol-level edge cases.

**Recency:** Highly relevant to current Go/Cosmos development standards.

**Source:** [ComeOnOliver/skillshub/skills/trailofbits/skills/cosmos-vulnerability-scanner/SKILL.md](https://github.com/ComeOnOliver/skillshub/blob/db216d3a3d5eef365d1ff27ef240f644e918f05a/skills/trailofbits/skills/cosmos-vulnerability-scanner/SKILL.md) · 52★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Cosmos Vulnerability Scanner

## 1. Purpose

Systematically scan Cosmos SDK blockchain modules and CosmWasm smart contracts for platform-specific security vulnerabilities that can cause chain halts, consensus failures, or fund loss. This skill encodes 9 critical vulnerability patterns unique to Cosmos-based chains.

## 2. When to Use This Skill

- Auditing Cosmos SDK modules (custom x/ modules)
- Reviewing CosmWasm smart contracts (Rust)
- Pre-launch security assessment of Cosmos chains
- Investigating chain halt incidents
- Validating consensus-critical code changes
- Reviewing ABCI method implementations

## 3. Platform Detection

### File Extensions & Indicators
- **Go files**: `.go`, `.proto`
- **CosmWasm**: `.rs` (Rust with cosmwasm imports)

### Language/Framework Markers
```go
// Cosmos SDK indicators
import (
    "github.com/cosmos/cosmos-sdk/types"
    sdk "github.com/cosmos/cosmos-sdk/types"
    "github.com/cosmos/cosmos-sdk/x/..."
)

// Common patterns
keeper.Keeper
sdk.Msg, GetSigners()
BeginBlocker, EndBlocker
CheckTx, DeliverTx
protobuf service definitions
```

```rust
// CosmWasm indicators
use cosmwasm_std::*;
#[entry_point]
pub fn execute(deps: DepsMut, env: Env,
```

</details>
