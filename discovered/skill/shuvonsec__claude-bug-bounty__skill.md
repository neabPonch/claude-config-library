---
name: shuvonsec__claude-bug-bounty__skill
source: https://github.com/shuvonsec/claude-bug-bounty/blob/22ea70b763618984a08d6f601bb2e3e079e86a15/skills/meme-coin-audit/SKILL.md
repo: shuvonsec/claude-bug-bounty
kind: skill
stars: 3143
last_pushed: 2026-06-12T17:51:53Z
license: mit
score: 9
domains: [security, blockchain, crypto]
tags: [audit, rug-pull, smart-contracts, forensics]
curated: 2026-06-15
curated_by: config-scout
---

# shuvonsec/claude-bug-bounty — skill

**Why it's worth keeping:** It contains precise, copy-pasteable grep commands that allow an agent to perform high-speed reconnaissance without reading every line of code. The 'Kill Signal' logic also provides a clear decision tree for the agent to minimize false positives.

**Summary:** A highly actionable security audit guide that provides structured reasoning frameworks and specific grep patterns for detecting rug pulls in EVM and Solana tokens.

**Source credibility:** Very high; 3k+ stars and active maintenance suggest it is a trusted security toolset.

**Recency:** Highly current, explicitly covering 2024-2025 risks like Solana's Token-2022 extensions.

**Source:** [shuvonsec/claude-bug-bounty/skills/meme-coin-audit/SKILL.md](https://github.com/shuvonsec/claude-bug-bounty/blob/22ea70b763618984a08d6f601bb2e3e079e86a15/skills/meme-coin-audit/SKILL.md) · 3143★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: meme-coin-audit
description: Meme coin and token security audit — rug pull detection (honeypot, hidden mint, fee manipulation, LP lock bypass), Solana SPL token analysis (freeze authority, mint authority, metadata mutability), Token-2022 extension risks (transfer hooks, permanent delegate), DEX liquidity pool attacks (sandwich amplification, LP drain, bonding curve exploits), pump.fun/Raydium/Jupiter integration risks, token_scanner.py automation, and real exploit examples from 2024-2025. Use for any token audit, rug pull assessment, meme coin security review, or pre-investment due diligence.
---

# MEME COIN & TOKEN SECURITY AUDIT

Fast-kill rug pull detection and deep token security analysis for EVM and Solana meme coins.

---

## PRE-DIVE KILL SIGNALS

Check these BEFORE reading a single line of code. If any are true, skip the audit — the token is likely a rug or not worth the time.

### Hard Kills (Skip Immediately)
- **Contract not verified** on Etherscan/Solscan → Cannot audit source = cannot trust
- **Deployer wallet** has history of rug pulls (check Etherscan deployer page)
- **Token age < 1 hour** AND no known team → Too early, wait for more data
- **Mint authori
```

</details>
