---
name: mozilla__fx-private-relay__skill
source: https://github.com/mozilla/fx-private-relay/blob/a6736286ded02ac6b30e9b681b8660fadbc00cce/.claude/skills/ble/SKILL.md
repo: mozilla/fx-private-relay
kind: skill
stars: 1741
last_pushed: 2026-06-15T19:13:41Z
license: other
score: 9
domains: [devops, sre, security-ops]
tags: [triage, on-call, automation]
curated: 2026-06-15
curated_by: config-scout
---

# mozilla/fx-private-relay — skill

**Why it's worth keeping:** It uses sophisticated patterns like environment dependency verification, dynamic time-window logic (handling Monday lookbacks), and explicit API field mappings to ensure high precision when interacting with external tools.

**Summary:** An operational playbook that automates daily SRE/on-call triage by scanning Slack, Jira, Sentry, and GitHub for a specific engineering team.

**Source credibility:** High; sourced from the official Mozilla Firefox Relay repository.

**Recency:** Current; integrates modern MCP server configurations and specific CLI tool dependencies.

**Source:** [mozilla/fx-private-relay/.claude/skills/ble/SKILL.md](https://github.com/mozilla/fx-private-relay/blob/a6736286ded02ac6b30e9b681b8660fadbc00cce/.claude/skills/ble/SKILL.md) · 1741★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ble
description: Run Base Load Engineer checks for the current day and produce a prioritized action list
tags: [relay, ble, ops, slack, sentry, jira, triage]
metadata:
  requires:
    mcpServers: ["slack", "plugin:atlassian:atlassian"]
---

# Base Load Engineer (BLE) Checks

## Prerequisites

Before running any checks, verify all dependencies are available. Run these
checks in parallel using Bash:

1. `which jq` — must be installed
2. `which gh` — must be installed
3. `gh auth status` — must be authenticated

If ANY dependency is missing, stop and output the following setup instructions
instead of running the BLE checks:

```
BLE skill setup required. Run these commands in your terminal:

# Install CLI tools (if missing)
brew install jq
brew install gh
gh auth login

# Add MCP servers (if not already configured)
claude mcp add --transport http --client-id 1601185624273.8899143856786 --callback-port 3118 slack https://mcp.slack.com/mcp
claude mcp add --transport http atlassian https://mcp.atlassian.com/v1/mcp

# Optional: auto-approve read-only MCP tools in .claude/settings.local.json
# Add these to permissions.allow to skip approval prompts:
#   "mcp__slack__slack_read_ch
```

</details>
