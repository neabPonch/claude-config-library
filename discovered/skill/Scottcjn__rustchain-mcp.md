---
name: Scottcjn__rustchain-mcp
source: https://github.com/Scottcjn/rustchain-mcp/blob/bab129dc5a13135488b2ded1c76d8dc68b529750/SKILL.md
repo: Scottcjn/rustchain-mcp
kind: skill
stars: 97
last_pushed: 2026-06-07T14:23:19Z
license: mit
score: 7
domains: [blockchain, agents-ai, cli-tools]
tags: [mcp, workflow-orchestration, blockchain]
curated: 2026-06-14
curated_by: config-scout
---

# Scottcjn/rustchain-mcp — skill

**Why it's worth keeping:** It moves beyond simple tool definitions to provide structured reasoning chains (Discovery → Analysis → Planning) that teach an agent how to chain tools effectively.

**Summary:** Defines strategic operational workflows for interacting with the RustChain blockchain, specifically targeting bounty hunting and wallet management.

**Source credibility:** Moderate; 97 stars indicates a recognized niche-specific tool with active development.

**Recency:** Current; follows modern MCP configuration standards.

**Source:** [Scottcjn/rustchain-mcp/SKILL.md](https://github.com/Scottcjn/rustchain-mcp/blob/bab129dc5a13135488b2ded1c76d8dc68b529750/SKILL.md) · 97★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# RustChain MCP Skill: Ecosystem Intelligence

This skill allows Claude Code to interact with the RustChain blockchain, monitor the network, and hunt for bounties.

## Setup

1. **Install the MCP Server**
   ```bash
   pip install rustchain-mcp
   ```

2. **Configure Claude Desktop/Code**
   Add the following to your configuration:
   ```json
   {
     "mcpServers": {
       "rustchain": {
         "command": "rustchain-mcp",
         "args": ["--api-key", "your-api-key"]
       }
     }
   }
   ```

## Tool-Based Workflows

### 1. Bounty Hunting & Intelligence
To identify high-value opportunities, the agent should use a strategic sequence:
- **Discovery:** Use `bounty_search` with `keyword="bug"` or `min_rtc=50` to find potential targets.
- **Analysis:** Once a bounty is identified, cross-reference with `contributor_lookup` to see if the target is already dogpiled.
- **Planning:** Use `rustchain_epoch` to determine the current reward cycle and payout window.

### 2. Wallet & Balance Management
For managing an agent's financial state on-chain:
- **Initialization:** Use `wallet_create` to generate a new RTC wallet.
- **Verification:** Use `wallet_balance` to check current holdings a
```

</details>
