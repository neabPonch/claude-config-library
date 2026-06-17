---
name: BillionsNetwork__verified-agent-identity
source: https://github.com/BillionsNetwork/verified-agent-identity/blob/f7ba72d001c91bb6dc1356a0064281e4dab6d730/SKILL.md
repo: BillionsNetwork/verified-agent-identity
kind: skill
stars: 754
last_pushed: 2026-05-18T09:34:12Z
license: unknown
score: 8
domains: [identity, security, blockchain-agents]
tags: [DID, authentication, guardrails, payment-automation]
curated: 2026-06-15
curated_by: config-scout
---

# BillionsNetwork/verified-agent-identity — skill

**Why it's worth keeping:** Employs a highly effective 'router table' for tool selection and implements strict cryptographic guardrails that prevent the agent from attempting unauthorized manual security workarounds.

**Summary:** A specialized skill framework for managing decentralized agent identities and automated x402 payment authentication.

**Source credibility:** High star count (754) suggests a recognized, used protocol within its niche.

**Recency:** Very recent; maintained within the last month.

**Source:** [BillionsNetwork/verified-agent-identity/SKILL.md](https://github.com/BillionsNetwork/verified-agent-identity/blob/f7ba72d001c91bb6dc1356a0064281e4dab6d730/SKILL.md) · 754★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: verified-agent-identity
description: Know Your Agent (KYA). Billions decentralized identity for agents. Link agents to human identities using Billions ERC-8004 and Attestation Registries. Verify and generate authentication proofs. Based on iden3 self-sovereign identity protocol.
metadata:
  {
    "category": "identity",
    "clawdbot":
      {
        "requires": { "bins": ["node"] },
        "config": { "optionalEnv": ["BILLIONS_NETWORK_MASTER_KMS_KEY"] },
      },
  }
homepage: https://billions.network/
---

## When to Use This Skill

This skill covers two capabilities. Read the **router table** below, then load the relevant reference before proceeding.

| Situation                                                               | Reference to load             |
| ----------------------------------------------------------------------- | ----------------------------- |
| Create, list, link, verify, or sign with a decentralized identity (DID) | `reference/identity/SKILL.md` |
| Handle a **402 Payment Required** HTTP response                         | `reference/x402/SKILL.md`     |

> **Always read the appropriate reference SKILL.md before running any script.**
> If a task
```

</details>
