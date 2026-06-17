---
name: grafana__gcx__skill
source: https://github.com/grafana/gcx/blob/74fff38ba3e8f7f9d7529ea7690fdfe905a1713a/claude-plugin/skills/investigate-alert/SKILL.md
repo: grafana/gcx
kind: skill
stars: 366
last_pushed: 2026-06-15T01:11:26Z
license: apache-2.0
score: 9
domains: [observability, devops, sre, cli-tools]
tags: [diagnostics, grafana, alerting]
curated: 2026-06-15
curated_by: config-scout
---

# grafana/gcx — skill

**Why it's worth keeping:** Implements a 'stop early' logic to prevent reporting on non-actionable states and provides structured templates for converting raw metrics into actionable insights like likely causes and next steps.

**Summary:** A high-density diagnostic workflow for investigating Grafana alerts that includes datasource correlation and error class categorization.

**Source credibility:** High; produced by the Grafana team for their official CLI tool.

**Recency:** Very recent/current; optimized for modern agentic command-line interactions.

**Source:** [grafana/gcx/claude-plugin/skills/investigate-alert/SKILL.md](https://github.com/grafana/gcx/blob/74fff38ba3e8f7f9d7529ea7690fdfe905a1713a/claude-plugin/skills/investigate-alert/SKILL.md) · 366★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: investigate-alert
description: Investigate Grafana alerts to determine why they are firing, their scope, and impact. Use when the user asks about a specific alert, wants to understand alert behavior, or needs to diagnose why an alert is in a firing or pending state.
---

# Grafana Alert Investigator

Investigate Grafana alerts by analyzing state, querying datasources, and identifying next steps. Be concise and direct - these are experienced operators who need actionable information, not hand-holding.

## Core Principles

1. Stop early for non-actionable scenarios (recording rules, healthy inactive alerts)
2. Be concise - no fluff, no excessive formatting, no obvious advice
3. Trust the user's expertise - no timelines, no patronizing suggestions
4. Focus on actionable information

## Prerequisites

User needs gcx installed with configured context and appropriate permissions. If gcx is not configured, use the setup-gcx skill first.

## Investigation Workflow

### Step 1: Verify Context and Locate Alert

Check context if needed (`gcx config view`). If multiple contexts exist and none specified, ask which to use.

### Step 2: Get Alert Details and Check for Early Exit

Fetch
```

</details>
