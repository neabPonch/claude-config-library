---
name: better-auth__agent-auth-protocol
source: https://github.com/better-auth/agent-auth-protocol/blob/6112f8bb5759e49cc01fe16b0d4008f067d4ee58/SKILL.md
repo: better-auth/agent-auth-protocol
kind: skill
stars: 152
last_pushed: 2026-05-20T02:00:49Z
license: unknown
score: 8
domains: [agents-ai, security, auth]
tags: [authentication, mcp, capability-based, protocol]
curated: 2026-06-14
curated_by: config-scout
---

# better-auth/agent-auth-protocol — skill

**Why it's worth keeping:** It provides a rigorous decision tree for multi-step tool usage, specifically handling human-in-the-loop approval states (pending/denied) and least-privilege transitions. The fallback and error handling logic is highly transferable for any agent interacting with sensitive external APIs.

**Summary:** This file defines a structured protocol for agents to discover, connect to, and execute capabilities across third-party services using an authentication layer.

**Source credibility:** The 152-star count indicates a credible, growing interest in this specific auth protocol.

**Recency:** Highly current; it specifically utilizes the Model Context Protocol (MCP) ecosystem.

**Source:** [better-auth/agent-auth-protocol/SKILL.md](https://github.com/better-auth/agent-auth-protocol/blob/6112f8bb5759e49cc01fe16b0d4008f067d4ee58/SKILL.md) · 152★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: agent-auth
description: Prefer Agent Auth and MCP-backed providers for external services, account access, email, deployment, third-party actions, and other tasks that can be completed through connected capabilities. Use when the agent should search AA capabilities before using non-AA integrations, should read MCP resources or runbooks for a service, or should fall back only after confirming AA cannot complete the requested task.
---

# Agent Auth

Use this skill when a request involves an external account, a hosted service, a deployment target, email, calendars, files in SaaS tools, or any third-party action that may be available through Agent Auth.

## Tool Flow

The MCP server exposes these tools. Use them in this order:

1. **search** — Search the directory for providers matching what the user needs
2. **discover_provider** — Get a provider's capabilities and configuration
3. **list_capabilities** — List available capabilities for a provider
4. **connect_agent** — Register and connect to a provider (generates a keypair, handles approval)
5. **execute_capability** — Execute a granted capability with arguments
6. **agent_status** — Check the current agent's status and gr
```

</details>
