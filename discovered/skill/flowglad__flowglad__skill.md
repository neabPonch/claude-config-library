---
name: flowglad__flowglad__skill
source: https://github.com/flowglad/flowglad/blob/aad66f18960bab4ca5f9f261ce26cd50b023283f/.claude/skills/pm/SKILL.md
repo: flowglad/flowglad
kind: skill
stars: 1716
last_pushed: 2026-05-17T18:12:00Z
license: other
score: 9
domains: [devops, sre, productivity, automation]
tags: [incident-response, slack-notion, postmortem]
curated: 2026-06-14
curated_by: config-scout
---

# flowglad/flowglad — skill

**Why it's worth keeping:** Excellent multi-step orchestration logic that includes data extraction schemas (Timeline/Root Cause) and specific MCP tool sequences like searching for database IDs before page creation.

**Summary:** Automates incident postmortems by extracting timeline and root cause data from Slack threads and documenting them in Notion.

**Source credibility:** High; sourced from a popular, well-maintained open-source repository.

**Recency:** Current; utilizes modern MCP patterns and structured agent reasoning.

**Source:** [flowglad/flowglad/.claude/skills/pm/SKILL.md](https://github.com/flowglad/flowglad/blob/aad66f18960bab4ca5f9f261ce26cd50b023283f/.claude/skills/pm/SKILL.md) · 1716★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pm
description: Create incident postmortems by reading Slack incident channels and creating structured postmortem documents in Notion. Use when conducting postmortem reviews or documenting incident responses.
---

# Incident Postmortem Generator

Create comprehensive incident postmortem documents by reading Slack incident channels and storing structured postmortems in Notion.

## When to Use

- After resolving a production incident
- When conducting postmortem reviews
- When documenting incident responses for team learning
- To generate action items from incident discussions

## Prerequisites

This skill requires the following MCP servers to be configured:
- **Slack MCP** - For reading incident channel history
- **Notion MCP** - For creating postmortem documents in the Notes database

Optional:
- **Betterstack MCP** - For including telemetry and uptime links

## Process

### 1. Identify the Incident Channel

Ask the user for the Slack channel name or ID. The channel should be the dedicated incident channel (typically named like `#incident-<name>` or `#inc-<date>-<description>`).

### 2. Read Slack Channel History

Use the Slack MCP to fetch the channel's message history:
```

</details>
