---
name: Cyfrin__audit-checklist__rareskill
source: https://github.com/Cyfrin/audit-checklist/blob/008855fe1798bbe75d86e6bf5f5e284b91bb2de6/ref/rareskill.md
repo: Cyfrin/audit-checklist
kind: skill
stars: 359
last_pushed: 2025-05-05T08:56:15Z
license: unknown
score: 8
domains: [security, smart-contracts, web3]
tags: [audit-checklist, solidity, evm, vulnerability-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# Cyfrin/audit-checklist — skill

**Why it's worth keeping:** It provides highly specific, advanced attack vectors (e.g., ERC777 griefing, signature malleability, oracle staleness) that move an agent beyond generic bug detection into expert-level protocol auditing.

**Summary:** A high-density security checklist specifically designed for auditing EVM smart contracts and Solidity code.

**Source credibility:** Very high; Cyfrin is a top-tier reputation in blockchain security and auditing.

**Recency:** Content is 14 months old, but core EVM/Solidity security principles remain highly relevant.

**Source:** [Cyfrin/audit-checklist/ref/rareskill.md](https://github.com/Cyfrin/audit-checklist/blob/008855fe1798bbe75d86e6bf5f5e284b91bb2de6/ref/rareskill.md) · 359★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Rareskill's Checklist (Extracted)

## Summary

**Author:**
[Jeffrey Scholz](https://www.linkedin.com/in/jeffreyscholz)

**Source:**
[Rareskill's Checklist](https://www.rareskills.io/post/smart-contract-security)

_The list below is a modified version extracted by [Nisedo](https://twitter.com/nisedo_)_

## Checklist

- Excessive function restriction
  - Getting the balance right
  - Security often boils down to managing the way money exits the contract
- Double voting or msg.sender spoofing
- Flashloan Governance Attacks
- Flashloan Price Attacks
- Bypassing the contract check
- tx.origin
- Gas Griefing or Denial of Service
  - Deleting arrays that others can add to is also an denial of service vector
  - ERC777, ERC721, and ERC1155 can also be griefing vectors
- Insecure Randomness
- Using the Chainlink Randomness Oracle Wrong
- Getting stale data from a price Oracle
- Relying on only one oracle
- Oracles in general are hard to get right
- Mixed accounting
- Treating cryptographic proofs like passwords
- Solidity does not upcast to the final uint size
- Solidity sneakily makes some literals uint8
- Solidity downcasting does not revert on overflow
- Writes to storage pointers don'
```

</details>
