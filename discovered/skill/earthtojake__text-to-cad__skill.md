---
name: earthtojake__text-to-cad__skill
source: https://github.com/earthtojake/text-to-cad/blob/1bca36b397f94abae08c96039b37ec1ee4969efe/skills/bambu-labs/SKILL.md
repo: earthtojake/text-to-cad
kind: skill
stars: 6408
last_pushed: 2026-06-13T21:23:43Z
license: mit
score: 9
domains: [hardware-control, cli-tools, iot]
tags: [3d-printing, bambu-lab, automation]
curated: 2026-06-15
curated_by: config-scout
---

# earthtojake/text-to-cad — skill

**Why it's worth keeping:** Uses 'execute' flags and explicit physical confirmation steps to prevent accidental hardware movement, and includes a detailed failure mode section that turns common errors into actionable troubleshooting instructions.

**Summary:** Provides highly specific automation logic for controlling Bambu Lab 3D printers over a local network using safety-first protocols. It manages the full lifecycle from configuration and status checks to file uploads and print execution.

**Source credibility:** High; part of a popular (6k+ stars) specialized repository with very recent activity.

**Recency:** Current; utilizes advanced agent orchestration patterns like tool handoffs ($cad-viewer) and strict execution requirements.

**Source:** [earthtojake/text-to-cad/skills/bambu-labs/SKILL.md](https://github.com/earthtojake/text-to-cad/blob/1bca36b397f94abae08c96039b37ec1ee4969efe/skills/bambu-labs/SKILL.md) · 6408★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: bambu-labs
description: Dry-run, upload, and cautiously initiate local Bambu Lab print jobs from validated plain `.gcode`, using Bambu LAN FTPS/MQTT handoffs.
---

# Bambu Labs

Provenance: maintained in [earthtojake/text-to-cad](https://github.com/earthtojake/text-to-cad).
Use the installed local skill files as the runtime source of truth; the
repository link is only for provenance and release review.

Use this skill for local-network Bambu Lab print handoffs after a plain `.gcode`
file already exists and has been validated. This skill does not slice models.

## Safety Rules

- Default to dry-run plans. Real printer traffic requires `--execute`.
- Never start a print without `--execute --confirm-start-print`.
- Pause and cancel controls are live printer requests; default to dry-run plans.
  Canceling a print requires `--execute --confirm-cancel-print`.
- Treat an explicit user request to print or start a specific job as live-start
  authorization; do not pause for a second confirmation solely for physical
  checks. Still validate the G-code, inspect the dry-run payload, read printer
  status, prefer upload-only before upload-start, state the physical checks, and
  stop i
```

</details>
