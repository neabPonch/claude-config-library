---
name: alsk1992__CloddsBot__skill
source: https://github.com/alsk1992/CloddsBot/blob/e71a5f635d99f453ef25ca1138d5f3ef7c4c686b/src/skills/bundled/endaoment/SKILL.md
repo: alsk1992/CloddsBot
kind: skill
stars: 392
last_pushed: 2026-06-12T19:40:36Z
license: mit
score: 8
domains: [blockchain, fintech, agents-ai]
tags: [web3, charity, smart-contracts, base]
curated: 2026-06-17
curated_by: config-scout
---

# alsk1992/CloddsBot — skill

**Why it's worth keeping:** It demonstrates how to provide essential technical constants—like smart contract addresses and EINs—within a skill file to prevent LLM hallucination. The use of 'gates' for private key security is an excellent pattern for sensitive financial operations.

**Summary:** Provides a specialized skill for an AI agent to facilitate USDC donations to 501(c)(3) charities on the Base network via Endaoment.

**Source credibility:** High; the source repository is well-starred, active, and specialized in AI agent commerce.

**Recency:** Current; follows the modern Claude Code skill specification.

**Source:** [alsk1992/CloddsBot/src/skills/bundled/endaoment/SKILL.md](https://github.com/alsk1992/CloddsBot/blob/e71a5f635d99f453ef25ca1138d5f3ef7c4c686b/src/skills/bundled/endaoment/SKILL.md) · 392★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: endaoment
description: "Donate to 501(c)(3) charities onchain via Endaoment - tax-deductible crypto donations"
command: donate
emoji: "💝"
gates:
  envs:
    - PRIVATE_KEY
---

# Endaoment Charity Donations

Donate to 501(c)(3) nonprofits onchain via Endaoment smart contracts on Base.

## Contracts (Base)

| Contract | Address |
|----------|---------|
| Registry | `0x237b53bcfbd3a114b549dfec96a9856808f45c94` |
| OrgFundFactory | `0x10fd9348136dcea154f752fe0b6db45fc298a589` |
| USDC | `0x833589fcd6edb6e08f4c7c32d4f71b54bda02913` |

## Commands

### Search
```
/donate search <name or EIN>     Find charity by name or EIN
/donate info <EIN>               Get charity info
```

### Donate
```
/donate <EIN> <amount>           Donate USDC to charity
/donate approve <amount>         Approve USDC for donations
```

## Popular Charities

| Charity | EIN |
|---------|-----|
| GiveDirectly | 27-1661997 |
| American Red Cross | 53-0196605 |
| Doctors Without Borders | 13-3433452 |
| ASPCA | 13-1623829 |

## Examples

```
/donate search "Red Cross"
/donate info 27-1661997
/donate 27-1661997 10              # Donate $10 USDC
```

## Fees

- Org donations: 1.5% fee (e.g., $100 → $1.50 fee,
```

</details>
