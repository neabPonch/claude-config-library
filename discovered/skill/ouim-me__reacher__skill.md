---
name: ouim-me__reacher__skill
source: https://github.com/ouim-me/reacher/blob/bf7d88438e72b0810f1de3a0ef4f66cafbb3020c/docs/skill.md
repo: ouim-me/reacher
kind: skill
stars: 26
last_pushed: 2026-04-01T20:59:10Z
license: mit
score: 8
domains: [agents-ai, devops, mcp-server]
tags: [setup-guide, installation-protocol, mcp]
curated: 2026-06-15
curated_by: config-scout
---

# ouim-me/reacher — skill

**Why it's worth keeping:** Uses a highly structured 'Ask-Check-Confirm' workflow that allows an agent to handle complex environment variables and security configurations autonomously.

**Summary:** An interactive setup protocol designed for AI agents to guide users through installing and configuring the Reacher MCP server.

**Source credibility:** Active project with recent updates and emerging community interest.

**Recency:** Highly current; specifically tailored for modern MCP and Claude Code workflows.

**Source:** [ouim-me/reacher/docs/skill.md](https://github.com/ouim-me/reacher/blob/bf7d88438e72b0810f1de3a0ef4f66cafbb3020c/docs/skill.md) · 26★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Reacher Setup Guide for AI Agents

This guide is for AI agents (Claude, etc.) helping a new user set up Reacher interactively. Walk through each step in order, asking for user input where needed.

The user does **not** need a VPS or Tailscale to get started. Confirm what they want before deciding which path to take.

---

## Step 1: Understand what the user wants

Ask the user:

> "What do you want Claude to be able to do? For example:
> - Call APIs on your behalf (GitHub, Linear, Notion, etc.)
> - Remember things across conversations (knowledge base)
> - Control a browser
> - SSH into your servers"

Based on their answer:
- **API + memory only** → Path 1 or 2 (no VPS or Tailscale needed)
- **+ SSH to machines** → Path 3 (needs Tailscale + VPS + SSH key)

---

## Step 2: Prerequisites check

**Always required:**
- Node.js 22+ — run `node --version` to check. Install from [nodejs.org](https://nodejs.org) if missing.
- A GitHub account — for `gist_kb` (knowledge base) and API calls to GitHub.

**Only for SSH features:**
- A [Tailscale](https://tailscale.com) account with devices enrolled
- A VPS or always-on machine with a public HTTPS URL

---

## Step 3: Clone and install

```bas
```

</details>
