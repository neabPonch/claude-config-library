---
name: vyqno__synthesis__nexus-skill
source: https://github.com/vyqno/synthesis/blob/39bf20156130423baabc4f56353520d5eda2fd03/nexus.skill.md
repo: vyqno/synthesis
kind: skill
stars: 1
last_pushed: 2026-03-21T15:12:40Z
license: unknown
score: 7
domains: [agents-ai, blockchain, mcp-servers]
tags: [autonomous-agent, multi-agent-orchestration, defi]
curated: 2026-06-14
curated_by: config-scout
---

# vyqno/synthesis — skill

**Why it's worth keeping:** It provides a high-quality structural blueprint: defining identity, tool discovery via CLI commands, clear service hierarchy (Orchestrator vs. Sub-agents), and specific operational guardrails.

**Summary:** An orchestration template for an autonomous agent that coordinates multiple specialized MCP servers and manages its own compute budget through DeFi yield.

**Source credibility:** Low social proof (1 star), but content depth suggests a sophisticated, non-generic experimental project.

**Recency:** Highly current; utilizes modern Claude CLI and MCP integration patterns.

**Source:** [vyqno/synthesis/nexus.skill.md](https://github.com/vyqno/synthesis/blob/39bf20156130423baabc4f56353520d5eda2fd03/nexus.skill.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Nexus — Master Skill File

## Identity

Nexus is an autonomous AI agent that earns its own compute budget from DeFi yield (Lido wstETH), funds inference via Bankr LLM gateway, and coordinates 6 specialized sub-agents. Every capability is exposed as an MCP server any AI can call.

**Agent:** nexus-agent.eth
**MCP Endpoint:** https://nexus-agent.xyz/mcp
**OpenClaw:** https://raw.githubusercontent.com/vyqno/synthesis/main/nexus.skill.md
**Identity:** ERC-8004 registered, ERC-8183 root, Self ZK verified

## When To Use Nexus

Use Nexus when you need:
- Lido staking operations (stake, unstake, wrap stETH)
- Autonomous trading (Uniswap swaps, GMX positions)
- Public goods evaluation (Octant scoring, Sybil resistance)
- ZK proof generation (Noir circuits, Lit TEE)
- Agent coordination (OpenServ, Olas, escrow)
- Treasury management (wstETH yield, Bankr billing)
- On-chain identity (ENS, ERC-8004, Self ZK, ERC-8128)
- Cross-chain operations (Base, Arbitrum, Celo, Ethereum)

## MCP Servers Available

| Server | Connect | Key Tools |
|---|---|---|
| nexus-lido-mcp | `python mcp/lido-mcp/server.py` | stake, unstake, get_vault_yield |
| nexus-treasury-mcp | `python mcp/treasury-mcp/server.py`
```

</details>
