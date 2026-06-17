---
name: jontsai__openclaw-command-center
source: https://github.com/jontsai/openclaw-command-center/blob/2fdb0c1213984558629886e15221681127504cd1/SKILL.md
repo: jontsai/openclaw-command-center
kind: skill
stars: 240
last_pushed: 2026-06-13T15:16:15Z
license: mit
score: 7
domains: [agents-ai, observability, cli-tools]
tags: [dashboard, monitoring, telemetry]
curated: 2026-06-14
curated_by: config-scout
---

# jontsai/openclaw-command-center — skill

**Why it's worth keeping:** Demonstrates how to use structured metadata to define skill installation requirements and local server execution paths, bridging the gap between an agent and full-stack observability.

**Summary:** Provides a mission control dashboard for real-time AI session monitoring, cost intelligence, and system vitals.

**Source credibility:** High; 240 stars and actively maintained by jontsai.

**Recency:** Current; last pushed within the current month.

**Source:** [jontsai/openclaw-command-center/SKILL.md](https://github.com/jontsai/openclaw-command-center/blob/2fdb0c1213984558629886e15221681127504cd1/SKILL.md) · 240★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: command-center
version: 1.4.1
description: Mission control dashboard for OpenClaw - real-time session monitoring, LLM usage tracking, cost intelligence, and system vitals. View all your AI agents in one place.
metadata:
  openclaw:
    requires:
      node: ">=18"
    install:
      - id: start
        kind: shell
        command: "node lib/server.js"
        label: "Start Command Center (http://localhost:3333)"
---

# OpenClaw Command Center

Mission control for your AI workforce.

## Quick Start

```bash
npx clawhub@latest install command-center
cd skills/command-center
node lib/server.js
```

Dashboard runs at **http://localhost:3333**

## Features

- **Session Monitoring** — Real-time view of all AI sessions with live updates
- **LLM Fuel Gauges** — Track Claude, Codex, and other model usage
- **System Vitals** — CPU, Memory, Disk, Temperature
- **Cron Jobs** — View and manage scheduled tasks
- **Cerebro Topics** — Automatic conversation organization
- **Cost Tracking** — Per-session costs, projections, savings estimates
- **Privacy Controls** — Hide sensitive topics for demos

## Configuration

The dashboard auto-detects your OpenClaw workspace. Set `OPENCLAW_WORKSPA
```

</details>
