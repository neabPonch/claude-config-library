---
name: garrytan__gbrain__skill
source: https://github.com/garrytan/gbrain/blob/090bb53203557f5659563ea28c1c847c32167aeb/skills/setup/SKILL.md
repo: garrytan/gbrain
kind: skill
stars: 22806
last_pushed: 2026-06-14T18:42:22Z
license: mit
score: 9
domains: [agents-ai, cli-tools, devops]
tags: [setup, provisioning, workflow-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# garrytan/gbrain — skill

**Why it's worth keeping:** It utilizes a 'Contract' to define success criteria and implements conditional logic (Phase A.5) to force user decisions on deployment shapes before proceeding.

**Summary:** A highly structured initialization skill for the GBrain agent system that manages infrastructure provisioning and architectural topology selection.

**Source credibility:** High; comes from a highly-starred, active repository with specific technical depth.

**Recency:** Current; uses modern toolchains like Bun, Supabase, and pgvector.

**Source:** [garrytan/gbrain/skills/setup/SKILL.md](https://github.com/garrytan/gbrain/blob/090bb53203557f5659563ea28c1c847c32167aeb/skills/setup/SKILL.md) · 22806★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: setup
description: Set up GBrain with auto-provision Supabase or PGLite, AGENTS.md injection, first import
triggers:
  - "set up gbrain"
  - "initialize brain"
  - "gbrain setup"
tools:
  - get_stats
  - get_health
  - sync_brain
  - put_page
mutating: true
---

# Setup GBrain

Set up GBrain from scratch. Target: working brain in under 5 minutes.

## Contract

- Setup completes with a working brain verified by `gbrain doctor --json` (all checks OK).
- The brain-first lookup protocol is injected into the project's AGENTS.md or equivalent.
- Live sync is configured and verified (a test change pushed and found via search).
- Schema state is tracked in `~/.gbrain/update-state.json` so future upgrades know what the user adopted or declined.
- No Supabase anon key is requested; GBrain uses only the database connection string.

## Install (if not already installed)

```bash
bun add github:garrytan/gbrain
```

## How GBrain connects

GBrain connects directly to Postgres over the wire protocol. NOT through the
Supabase REST API. You need the **database connection string** (a `postgresql://` URI),
not the project URL or anon key. The password is embedded in the connection string.
```

</details>
