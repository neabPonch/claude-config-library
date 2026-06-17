---
name: aspectrr__deer__skill
source: https://github.com/aspectrr/deer/blob/e4f98458be4066648e4e3e1a5440e83a4e18f70f/deer-cli/internal/skill/defaults/kibana-alerting-rules/SKILL.md
repo: aspectrr/deer
kind: skill
stars: 405
last_pushed: 2026-04-21T12:56:18Z
license: mit
score: 9
domains: [devops, observability, infrastructure-as-code]
tags: [kibana, elasticsearch, alerting, api-management]
curated: 2026-06-16
curated_by: config-scout
---

# aspectrr/deer — skill

**Why it's worth keeping:** Includes high-value 'Common Pitfalls' and 'Best Practices' that prevent common errors like missing XSRF headers; provides both API and Terraform examples for multi-modal workflows.

**Summary:** Provides full lifecycle management for Kibana alerting rules via REST API and Terraform. Includes necessary authentication headers, endpoint mappings, and rule schema details.

**Source credibility:** High quality; comes from a specialized tool (deer) with significant GitHub stars.

**Recency:** Highly current, with updates within the last two months.

**Source:** [aspectrr/deer/deer-cli/internal/skill/defaults/kibana-alerting-rules/SKILL.md](https://github.com/aspectrr/deer/blob/e4f98458be4066648e4e3e1a5440e83a4e18f70f/deer-cli/internal/skill/defaults/kibana-alerting-rules/SKILL.md) · 405★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: kibana-alerting-rules
description: >
  Create and manage Kibana alerting rules via REST API or Terraform. Use when creating,
  updating, or managing rule lifecycle (enable, disable, mute, snooze) or rules-as-code
  workflows.
metadata:
  author: elastic
  version: 0.1.0
  source: elastic/agent-skills//skills/kibana/kibana-alerting-rules
---

# Kibana Alerting Rules

## Core Concepts

A rule has three parts: **conditions** (what to detect), **schedule** (how often to check), and **actions** (what
happens when conditions are met). When conditions are met, the rule creates **alerts**, which trigger **actions** via
**connectors**.

## Authentication

All alerting API calls require either API key auth or Basic auth. Every mutating request must include the `kbn-xsrf`
header.

```http
kbn-xsrf: true
```

## API Reference

Base path: `<kibana_url>/api/alerting` (or `/s/<space_id>/api/alerting` for non-default spaces).

| Operation         | Method | Endpoint                                                   |
| ----------------- | ------ | ---------------------------------------------------------- |
| Create rule       | POST   | `/api/alerting/rule/{id}`
```

</details>
