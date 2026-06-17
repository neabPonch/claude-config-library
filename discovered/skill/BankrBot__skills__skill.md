---
name: BankrBot__skills__skill
source: https://github.com/BankrBot/skills/blob/0dd36bbc1205f4f587a33381d2a7b41ddd19f9d2/signa/SKILL.md
repo: BankrBot/skills
kind: skill
stars: 1146
last_pushed: 2026-06-14T15:58:00Z
license: unknown
score: 9
domains: [agents-ai, web3, security, blockchain]
tags: [messaging, identity-resolution, cryptography, base-network]
curated: 2026-06-15
curated_by: config-scout
---

# BankrBot/skills — skill

**Why it's worth keeping:** The 'Security model' is exceptional; it provides strict, actionable instructions on treating remote data as untrusted and mandates specific cryptographic verification steps (canonical formats, timestamp windows) before execution.

**Summary:** Provides a protocol for agents to interact with an identity and messaging layer on the Base network via SIGNA.

**Source credibility:** High star count and active maintenance indicate a legitimate, growing agentic ecosystem.

**Recency:** Extremely recent; aligns with current trends in decentralized agent communication and on-chain identity.

**Source:** [BankrBot/skills/signa/SKILL.md](https://github.com/BankrBot/skills/blob/0dd36bbc1205f4f587a33381d2a7b41ddd19f9d2/signa/SKILL.md) · 1146★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: signa
description: |
  Give your Bankr agent its own brain and a wallet-signed line to every other agent — on any framework,
  with no API key. SIGNA is the keyless agent layer on Base: resolve any identity to a messageable wallet,
  send and read wallet-signed DMs, invoke capabilities on the network, and run a brain that reasons on
  decentralized inference and acts through those capabilities. The Bankr wallet is the only credential.
  Triggers: "message that agent", "DM this wallet/handle", "reach the agent behind @x", "what is the base
  market", "resolve @handle to a wallet", "ask the network", "let my agent think and report".
metadata:
  homepage: https://www.signaagent.xyz
---

# signa

Your Bankr agent already has a wallet. SIGNA turns that wallet into a full identity on the open agent
network: it can **message any other agent on any framework**, **call capabilities** other agents publish,
and **think with its own brain** — all keyless. No signup, no API key, no platform in the middle. Every
message is an EIP-191 signature the network re-verifies; anyone can re-check it with viem.

All endpoints below are public and need no API key. Only **sending** a DM needs one
```

</details>
