---
name: VenusProtocol__oracle
source: https://github.com/VenusProtocol/oracle/blob/aed5f330a3705b22723ea0de50d4460edd6dffc4/CLAUDE.md
repo: VenusProtocol/oracle
kind: claude-md
stars: 19
last_pushed: 2026-06-15T06:55:23Z
license: bsd-3-clause
score: 9
domains: [smart-contracts, blockchain, security]
tags: [solidity, hardhat, defi, oracle]
curated: 2026-06-15
curated_by: config-scout
---

# VenusProtocol/oracle — claude-md

**Why it's worth keeping:** It includes critical behavioral guardrails (security rigor) and explains the relationship between key contracts to prevent logic errors during refactoring.

**Summary:** Provides high-stakes context for a DeFi oracle system, including architectural mental models and rigorous security/testing protocols.

**Source credibility:** High; Venus Protocol is a prominent DeFi protocol with active maintenance.

**Recency:** Current; includes modern Solidity versions and sophisticated Hardhat/testing workflows.

**Source:** [VenusProtocol/oracle/CLAUDE.md](https://github.com/VenusProtocol/oracle/blob/aed5f330a3705b22723ea0de50d4460edd6dffc4/CLAUDE.md) · 19★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Venus Protocol Oracle — Solidity smart contract project using Hardhat.

This is a DeFi protocol handling real funds. Always write clean, secure code — never apply quick patches or workarounds without understanding all side effects. Verify the impact of every change across the codebase. Every task deserves the same level of rigour; nothing should be treated as low priority or left at low quality. Never assume — if in doubt, ask and confirm before proceeding.

---

## Package Manager

Use **yarn** — never use npm.

```bash
yarn install                   # install dependencies
```

---

## Common Commands

```bash
yarn compile                   # compile contracts (regular + zksync)
yarn build                     # full build (tsc + hardhat compile + copy artifacts)
yarn test                      # compile + run all tests
npx hardhat test <file>        # run a specific test file
yarn lint                      # ESLint + Prettier + Solhint check
yarn prettier                  # auto-format code
yarn docgen                    # generate contract docs
```

### Fork Tests

```bash
# Requires FORK=true + FORKED_NETWORK + ARCHIVE_NODE_<network> in .env
FORK=true FORKED_NETWORK=
```

</details>
