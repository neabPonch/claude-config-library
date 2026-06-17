---
name: nickyreinert__meMCP__memcp-skill
source: https://github.com/nickyreinert/meMCP/blob/53dba148ccc11f705d1d54d4404f5a2fd8f43f92/skills/meMCP-SKILL.md
repo: nickyreinert/meMCP
kind: skill
stars: 7
last_pushed: 2026-02-26T21:21:14Z
license: unknown
score: 8
domains: [api-interaction, cli-tools, agentic-workflows]
tags: [rest-api, bash, automation]
curated: 2026-06-16
curated_by: config-scout
---

# nickyreinert/meMCP — skill

**Why it's worth keeping:** It provides excellent patterns for documenting access tiers (public vs admin), specific business workflows, and instructions on how to bridge the gap between an LLM and an API using curl/bash tools.

**Summary:** A highly structured skill for interacting with a personal profile REST API via shell commands.

**Source credibility:** Moderate; 7 stars on GitHub and shows recent activity in terms of development cycle.

**Recency:** Current; it addresses the practical need for agents to use shell-based HTTP clients (curl) to interact with external services.

**Source:** [nickyreinert/meMCP/skills/meMCP-SKILL.md](https://github.com/nickyreinert/meMCP/blob/53dba148ccc11f705d1d54d4404f5a2fd8f43f92/skills/meMCP-SKILL.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: meMCP
description: >
  Connect to and interact with a meMCP server — a personal MCP profile server
  (github.com/nickyreinert/meMCP) that serves professional profile data including career
  stages, projects, articles, skills, and technologies. Use this skill whenever the user
  wants to query, explore, create, or manage data on their meMCP server. Triggers include:
  "talk to my meMCP", "query my profile server", "create an interview", "add a project",
  "search my skills", "what's on my meMCP", "use my MCP server", "meMCP", or any mention
  of interacting with a personal profile/portfolio API server with token auth.
---

# meMCP Skill

Interact with a running meMCP server — a FastAPI-based personal profile MCP server.

## Setup: Required Configuration

Before doing anything, ask the user for these if not already provided in the conversation:

1. **Server URL** — e.g. `http://localhost:8000` or `https://mymcp.example.com`
2. **Token** — for protected endpoints (admin or elevated access token from `config.tech.yaml`)

Store these mentally for the session. Never hardcode them in output.

---

## Access Tiers

meMCP has three access tiers:

| Tier | Token Required | Examples
```

</details>
