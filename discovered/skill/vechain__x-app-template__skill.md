---
name: vechain__x-app-template__skill
source: https://github.com/vechain/x-app-template/blob/8692b6a3b0e8d5cc18d3039988fa5d3612f7517c/.agents/skills/vechain-react-native-dev/SKILL.md
repo: vechain/x-app-template
kind: skill
stars: 446
last_pushed: 2026-06-13T13:41:48Z
license: unknown
score: 9
domains: [blockchain-integration, mobile-development, react-native]
tags: [web3, react-native, vechain, deep-linking]
curated: 2026-06-15
curated_by: config-scout
---

# vechain/x-app-template — skill

**Why it's worth keeping:** It employs advanced agent-steering techniques like information priority hierarchy (Reference > MCP > Web) and captures critical low-level implementation requirements like specific crypto import orders.

**Summary:** A highly specialized protocol for an AI agent to assist in developing React Native dApps that integrate with VeWorld wallets.

**Source credibility:** High; official template from the VeChain organization with recent maintenance.

**Recency:** Current; integrates modern concepts like MCP tools and specific Node/React Native environmental constraints.

**Source:** [vechain/x-app-template/.agents/skills/vechain-react-native-dev/SKILL.md](https://github.com/vechain/x-app-template/blob/8692b6a3b0e8d5cc18d3039988fa5d3612f7517c/.agents/skills/vechain-react-native-dev/SKILL.md) · 446★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: vechain-react-native-dev
description: React Native VeWorld wallet integration — deep link communication, NaCl encryption, transaction signing, certificate signing, EIP-712 typed data, and multi-network support.
allowed-tools: []
license: MIT
metadata:
  author: VeChain
  version: "0.1.0"
---

# React Native Wallet Link Skill

## CRITICAL RULES

1. **Read reference files FIRST.** When the user's request involves any topic in the reference table below, read those files before doing anything else — before writing code, before making decisions. Briefly mention which files you are reading so the user can confirm the skill is active (e.g., "Reading wallet link API reference...").
2. **Information priority for VeChain topics:** (a) Reference files in this skill — always the primary source. (b) VeChain MCP tools — use `@vechain/mcp-server` for on-chain data, transaction building, and live network queries; use Kapa AI MCP for VeChain documentation lookups. (c) Web search — only as a last resort, and only for topics NOT covered in the reference files.
3. **Prefer working directly in the main conversation** for VeChain tasks. Plan mode and subagents do not inherit skill context and
```

</details>
