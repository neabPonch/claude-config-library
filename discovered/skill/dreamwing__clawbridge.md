---
name: dreamwing__clawbridge
source: https://github.com/dreamwing/clawbridge/blob/752b03ac2ca38da6afba487f4508ba85f1377428/SKILL.md
repo: dreamwing/clawbridge
kind: skill
stars: 233
last_pushed: 2026-03-18T17:23:55Z
license: unknown
score: 8
domains: [agents-ai, devops, monitoring]
tags: [dashboard, sidecar, node.js]
curated: 2026-06-15
curated_by: config-scout
---

# dreamwing/clawbridge — skill

**Why it's worth keeping:** Provides an excellent blueprint for managing credentials (auto-generated .env) and network security (explicit inbound/outbound requirements). It also demonstrates how to implement persistent background services using systemd.

**Summary:** A manifest for a Node.js sidecar dashboard used to monitor agent thoughts, costs, and tasks via a mobile-friendly web UI.

**Source credibility:** High; part of a recognized open-source project with significant community engagement (233 stars).

**Recency:** Current; last updated within the last 3 months.

**Source:** [dreamwing/clawbridge/SKILL.md](https://github.com/dreamwing/clawbridge/blob/752b03ac2ca38da6afba487f4508ba85f1377428/SKILL.md) · 233★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
<skill>
  <id>clawbridge</id>
  <name>ClawBridge Dashboard</name>
  <version>1.0.0</version>
  <description>Mobile-first mission control for OpenClaw agents. Runs as a local Node.js sidecar process, providing a web dashboard to monitor real-time agent activity, track token costs across 340+ models, and trigger cron tasks remotely. Optionally creates an outbound-only Cloudflare tunnel for remote access.</description>
  <author>DreamWing</author>
  <homepage>https://clawbridge.app</homepage>
  <license>MIT</license>
  <tags>dashboard,monitoring,mobile,ui,control-panel,cost-tracking,cloudflare,tunnel</tags>

  <!-- What this skill installs and runs -->
  <runtime>
    <type>node</type>
    <entrypoint>index.js</entrypoint>
    <persistence>Registers a user-level systemd service (clawbridge.service) that auto-starts on login and restarts on failure.</persistence>
  </runtime>

  <!-- System requirements -->
  <requires>
    <dependency name="node" version=">=18" required="true" />
    <dependency name="npm" version=">=9" required="true" />
    <dependency name="git" version="any" required="false" description="Used for incremental updates; falls back to tarball download if absent." />
```

</details>
