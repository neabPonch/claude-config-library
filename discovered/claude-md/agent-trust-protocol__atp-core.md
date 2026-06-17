---
name: agent-trust-protocol__atp-core
source: https://github.com/agent-trust-protocol/atp-core/blob/73be6a6658a3417ca041ae2e6937488a266dba7b/CLAUDE.md
repo: agent-trust-protocol/atp-core
kind: claude-md
stars: 2
last_pushed: 2026-06-14T19:41:58Z
license: apache-2.0
score: 8
domains: [agents-ai, security, cli-tools]
tags: [agentic-workflows, mcp, task-planning, knowledge-management]
curated: 2026-06-15
curated_by: config-scout
---

# agent-trust-protocol/atp-core — claude-md

**Why it's worth keeping:** Demonstrates advanced techniques for mandatory step sequencing (e.g., 'MUST call X before Y') to ensure state persistence and reliability during complex tasks.

**Summary:** Combines project architecture with highly structured, rule-based agent workflows for tool interaction and memory management.

**Source credibility:** Low star count indicates an early/niche project, but the content reflects high-level agent orchestration logic.

**Recency:** Highly current; integrates workflows specifically designed for the Model Context Protocol (MCP).

**Source:** [agent-trust-protocol/atp-core/CLAUDE.md](https://github.com/agent-trust-protocol/atp-core/blob/73be6a6658a3417ca041ae2e6937488a266dba7b/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# === USER INSTRUCTIONS ===
[byterover-mcp]

[byterover-mcp]

# Byterover MCP Server Tools Reference

There are two main workflows with Byterover tools and recommended tool call
strategies that you **MUST** follow precisely.

## Onboarding workflow
If users particularly ask you to start the onboarding process, you **MUST
STRICTLY** follow these steps.
1. **ALWAYS USE** **byterover-check-handbook-existence** first to check if the
byterover handbook already exists. If not, You **MUST** call
**byterover-create-handbook** to create the byterover handbook.
2. If the byterover handbook already exists, first you **MUST** USE
**byterover-check-handbook-sync** to analyze the gap between the current
codebase and the existing byterover handbook.
3. Then **IMMEDIATELY USE** **byterover-update-handbook** to update these
changes to the byterover handbook.
4. During the onboarding, you **MUST** use **byterover-list-modules** **FIRST**
to get the available modules, and then **byterover-store-modules** and
**byterover-update-modules** if there are new modules or changes to existing
modules in the project.

## Planning workflow
Based on user request, you **MUST** follow these sequences of tool calls
```

</details>
