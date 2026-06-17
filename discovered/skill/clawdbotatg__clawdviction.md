---
name: clawdbotatg__clawdviction
source: https://github.com/clawdbotatg/clawdviction/blob/da4fa15d06f4dd3f3e4ec0b89fd22d60603314bc/skill.md
repo: clawdbotatg/clawdviction
kind: skill
stars: 3
last_pushed: 2026-05-27T01:48:59Z
license: mit
score: 9
domains: [blockchain, web3-agents, cli-tools]
tags: [ethereum, staking, abi-provided, onchain-governance]
curated: 2026-06-14
curated_by: config-scout
---

# clawdbotatg/clawdviction — skill

**Why it's worth keeping:** Includes raw ABIs for direct function invocation and explicit mathematical formulas to convert raw onchain values into human-readable formats.

**Summary:** A high-density domain-specific context file that enables an AI agent to interact with a blockchain ecosystem via RPC calls or CLI tools.

**Source credibility:** Low star count, but the high technical specificity of the contract interactions suggests it is a functional project file.

**Recency:** Current; includes modern protocol references like Base chain and Uniswap v4.

**Source:** [clawdbotatg/clawdviction/skill.md](https://github.com/clawdbotatg/clawdviction/blob/da4fa15d06f4dd3f3e4ec0b89fd22d60603314bc/skill.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# larv.ai — AI Agent Skill File

Everything an AI agent needs to interact with the larv.ai ecosystem programmatically.

## Chain & Contracts

- **Chain:** Base (chainId `8453`)
- **RPC:** `https://mainnet.base.org`
- **$CLAWD Token:** `0x9f86dB9fc6f7c9408e8Fda3Ff8ce4e78ac7a6b07` (ERC-20, 18 decimals)
- **ClawdVictionStaking:** `0xC9E377FB98a1aA6Ecf4B553cE1b57940121213bf`

## How to Stake

### 1. Approve

Call `approve(spender, amount)` on the $CLAWD token contract.

- `spender`: `0xC9E377FB98a1aA6Ecf4B553cE1b57940121213bf`
- `amount`: token amount in wei (human amount × 1e18)

### 2. Stake

Call `stake(uint256 amount)` on the staking contract.

- Minimum: 1,000 CLAWD (`1000000000000000000000` wei)
- Tokens transfer from your wallet to the contract

### 3. Check Your Stake

- `getActiveStakes(address user)` → returns arrays of amounts and timestamps
- `getClawdviction(address user)` → returns raw CV (divide by `1728000e18` for human-readable)

### 4. Unstake

Call `unstake(uint256 stakeIndex)` with the index of the position to unstake.

- Tokens return immediately, no lockup
- Unstaking resets conviction for that position

## Conviction (CV) Mechanics

```
clawdviction = amount_stak
```

</details>
