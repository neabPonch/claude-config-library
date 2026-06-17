---
name: jiayaoqijia__cryptoskill__skill
source: https://github.com/jiayaoqijia/cryptoskill/blob/f735d925dde61be9de49edae86289b4f9e57175e/skills/chains/solidity/SKILL.md
repo: jiayaoqijia/cryptoskill
kind: skill
stars: 61
last_pushed: 2026-06-04T03:32:35Z
license: agpl-3.0
score: 8
domains: [smart-contracts, security, blockchain]
tags: [solidity, ethereum, web3, security-audit]
curated: 2026-06-15
curated_by: config-scout
---

# jiayaoqijia/cryptoskill — skill

**Why it's worth keeping:** The 'Pitfall -> Best Practice' structure is ideal for LLM instruction; it includes specific technical details like EIP-1967 slots and visibility nuances that prevent common vulnerabilities.

**Summary:** Provides high-density security and efficiency rules for Solidity development. It covers critical patterns like Reentrancy protection, gas optimization, and upgradeable contract storage.

**Source credibility:** Decent niche reputation with 61 stars for a specialized skills repository.

**Recency:** Very current, as the content covers modern Solidity (0.8+) and essential security standards.

**Source:** [jiayaoqijia/cryptoskill/skills/chains/solidity/SKILL.md](https://github.com/jiayaoqijia/cryptoskill/blob/f735d925dde61be9de49edae86289b4f9e57175e/skills/chains/solidity/SKILL.md) · 61★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: Solidity
description: Avoid common Solidity mistakes — reentrancy, gas traps, storage collisions, and security pitfalls.
metadata: {"clawdbot":{"emoji":"⟠","os":["linux","darwin","win32"]}}
---

## Reentrancy
- External calls before state updates — attacker can re-enter before state changes
- Checks-Effects-Interactions pattern — validate, update state, THEN external call
- `ReentrancyGuard` from OpenZeppelin — use `nonReentrant` modifier on vulnerable functions
- `transfer()` and `send()` have 2300 gas limit — but don't rely on this for security

## Integer Handling
- Solidity 0.8+ reverts on overflow — but `unchecked {}` blocks bypass this
- Division truncates toward zero — `5 / 2 = 2`, no decimals
- Use fixed-point math for precision — multiply before divide, or use libraries
- `type(uint256).max` for max value — don't hardcode large numbers

## Gas Gotchas
- Unbounded loops can exceed block gas limit — paginate or limit iterations
- Storage writes cost 20k gas — memory/calldata much cheaper
- `delete` refunds gas but has limits — refund capped, don't rely on it
- Reading storage in loop — cache in memory variable first

## Visibility and Access
- State variables defau
```

</details>
