---
name: protokol__solidity-typescript-hardhat-template__skill
source: https://github.com/protokol/solidity-typescript-hardhat-template/blob/158b5ede035c31f6cc5227b48f63c9126cc08a09/.claude/skills/new-contract/SKILL.md
repo: protokol/solidity-typescript-hardhat-template
kind: skill
stars: 48
last_pushed: 2026-04-08T15:48:44Z
license: mit
score: 8
domains: [blockchain, smart-contracts, web3-development]
tags: [solidity, hardhat, scaffolding, testing]
curated: 2026-06-16
curated_by: config-scout
---

# protokol/solidity-typescript-hardhat-template — skill

**Why it's worth keeping:** Enforces strict adherence to specific architectural patterns (OpenZeppelin v5, Hardhat Ignition) across multiple files. It handles essential side effects like task registration and verification steps that are often missed during manual development.

**Summary:** Automates the complete scaffolding of a Solidity feature including contracts, tests, deployment modules, and Hardhat tasks.

**Source credibility:** Moderate star count for a niche template; recent activity suggests it is well-maintained.

**Recency:** Highly current, referencing modern standards like Hardhat v3 and OpenZeppelin v5.

**Source:** [protokol/solidity-typescript-hardhat-template/.claude/skills/new-contract/SKILL.md](https://github.com/protokol/solidity-typescript-hardhat-template/blob/158b5ede035c31f6cc5227b48f63c9126cc08a09/.claude/skills/new-contract/SKILL.md) · 48★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
description: Scaffold a new Solidity contract with test, Ignition module, and tasks following project patterns
user-invocable: true
disable-model-invocation: true
---

# /new-contract

Scaffold a new Solidity contract following the project's existing patterns.

## Instructions

1. **Ask the user** for:
    - Contract name (PascalCase, e.g., `MyToken`)
    - Token standard (ERC20, ERC721, ERC1155, or custom)
    - Features needed (Ownable, Pausable, Burnable, etc.)

2. **Create the contract** in `contracts/<ContractName>.sol`:
    - Use `pragma solidity 0.8.28;`
    - Import from `@openzeppelin/contracts/`
    - Follow the patterns in existing contracts (e.g., `BasicERC20.sol`)
    - Pass `initialOwner` to `Ownable` constructor (OpenZeppelin v5 pattern)
    - Include SPDX-License-Identifier: MIT

3. **Create the test file** in `test/<ContractName>.ts`:
    - Use the `setupFixture` + `loadFixture` pattern from existing tests
    - Use top-level `await hre.network.connect()` for ethers/networkHelpers
    - Test constructor parameters, core functionality, and access control
    - Use `revertedWithCustomError` for OpenZeppelin error assertions

4. **Create the Ignition module** in `
```

</details>
