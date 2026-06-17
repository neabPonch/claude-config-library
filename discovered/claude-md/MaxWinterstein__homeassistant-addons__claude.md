---
name: MaxWinterstein__homeassistant-addons__claude
source: https://github.com/MaxWinterstein/homeassistant-addons/blob/668a5c2694f764bbe400e18f5f5075942e376ffa/planefence/CLAUDE.md
repo: MaxWinterstein/homeassistant-addons
kind: claude-md
stars: 169
last_pushed: 2026-06-11T21:02:41Z
license: gpl-3.0
score: 8
domains: [devops, cli-tools, embedded-systems]
tags: [shell-scripting, containerization, versioning-rules]
curated: 2026-06-15
curated_by: config-scout
---

# MaxWinterstein/homeassistant-addons — claude-md

**Why it's worth keeping:** It provides highly specific technical guardrails, such as the required custom shebang and preferred string substitution methods, which prevents an AI from introducing non-idiomatic code.

**Summary:** Defines strict operational constraints for versioning, service startup sequences, and project-specific shell scripting idioms.

**Source credibility:** High; part of a specialized, actively maintained Home Assistant addon repository.

**Recency:** Current; reflects modern containerized deployment patterns and shell environment requirements.

**Source:** [MaxWinterstein/homeassistant-addons/planefence/CLAUDE.md](https://github.com/MaxWinterstein/homeassistant-addons/blob/668a5c2694f764bbe400e18f5f5075942e376ffa/planefence/CLAUDE.md) · 169★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Planefence Add-on — Claude Instructions

## Versioning

- Bump the **patch version** in `config.yaml` and `CHANGELOG.md` on **every single commit**
- Version format: `MAJOR.MINOR.PATCH` — only bump patch for fixes/tweaks, minor for new features
- The `image:` line in `config.yaml` stays **commented out** so the addon builds locally from the Dockerfile during development

## Architecture

- `export-env-from-config.sh` — sourced by cont-init; exports `/data/options.json` as env vars, resolves `HOMEASSISTANT_LATITUDE`/`LONGITUDE` placeholders via HA Supervisor API
- `rootfs/etc/cont-init.d/00-ha-planefence-config.sh` — writes resolved options into `planefence.config` before s6 services start; signals readiness via `/run/ha-planefence-ready`
- The Dockerfile patches upstream s6 scripts to wait for `/run/ha-planefence-ready` before reading config

## Shell scripting

- Scripts run under `#!/usr/bin/with-contenv bashio` which enables `set -e` and `set -o pipefail` — always add `|| true` to commands that are allowed to fail (e.g. DNS lookups, optional checks)
- Use bash string substitution (`${var//old/new}`) instead of `sed` for simple replacements inside variables
- The `set_config()`
```

</details>
