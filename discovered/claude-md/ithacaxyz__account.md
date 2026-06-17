---
name: ithacaxyz__account
source: https://github.com/ithacaxyz/account/blob/767e973ad2a083aa3231a88b2472055d6c556307/CLAUDE.md
repo: ithacaxyz/account
kind: claude-md
stars: 322
last_pushed: 2026-01-03T20:20:58Z
license: mit
score: 9
domains: [blockchain, smart-contracts]
tags: [solidity, foundry, security, gas-optimization]
curated: 2026-06-15
curated_by: config-scout
---

# ithacaxyz/account — claude-md

**Why it's worth keeping:** Uses concrete 'Do vs. Don't' code examples for error handling and reentrancy, and includes specific CLI commands for gas benchmarking and test verification.

**Summary:** Provides high-precision Solidity development standards covering gas optimization, security patterns like CEI/reentrancy protection, and Foundry testing workflows.

**Source credibility:** High-quality open-source project with significant star count and recent maintenance.

**Recency:** Highly current, utilizing modern Foundry/Solidity standards.

**Source:** [ithacaxyz/account/CLAUDE.md](https://github.com/ithacaxyz/account/blob/767e973ad2a083aa3231a88b2472055d6c556307/CLAUDE.md) · 322★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Solidity Contribution Guidelines

### 1. General Principles

- **Think first, code second**: Minimize the number of lines changed and consider ripple effects across the codebase.
- **Prefer simplicity**: Fewer moving parts ➜ fewer bugs and lower audit overhead.

### 2. Assembly Usage

| Rule | Rationale |
|------|-----------|
| Use assembly only when essential. | Keeps code readable and auditable. |
| Assembly is mandatory for low-level external calls. | Gives full control over call parameters & return data, and saves gas. |
| Precede every assembly block with: • A brief justification (1-2 lines). • Equivalent Solidity pseudocode. | Documents intent for reviewers. |
| Mark assembly blocks memory-safe when the Solidity docs' criteria are met. | Enables compiler optimizations. |

### 3. Gas Optimization

- Keep a dedicated **Gas Optimization** section in the PR description; justify any measurable gas deltas.
- Prefer `calldata` over `memory` for function arguments wherever possible, as `calldata` is cheaper. Note that `calldata` is read-only.
- Limit storage (`sstore`, `sload`) operations; cache in memory wherever possible.
- Use forge snapshot, forge test --match-test "benchmark"
```

</details>
