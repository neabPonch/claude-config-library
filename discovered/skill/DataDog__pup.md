---
name: DataDog__pup
source: https://github.com/DataDog/pup/blob/652a6fd2f35428c719347715025a4e6168be4607/SKILL.md
repo: DataDog/pup
kind: skill
stars: 893
last_pushed: 2026-06-12T20:39:55Z
license: apache-2.0
score: 9
domains: [cli-tools, devops, infrastructure]
tags: [modular-skills, datadog, agentic-workflow]
curated: 2026-06-14
curated_by: config-scout
---

# DataDog/pup — skill

**Why it's worth keeping:** Uses the 'Domain Agent' pattern to prevent context window bloat; instead of one giant toolset, it provides high-precision modules (e.g., dd-logs, dd-apm) for specific intents.

**Summary:** A modular skill distribution system that decomposes complex Datadog API capabilities into specialized domain-specific agents.

**Source credibility:** High; authored by Datadog, a major infrastructure player with an actively maintained CLI.

**Recency:** Highly current; includes modern workflows for injecting skills into AI assistants like Claude and Cursor.

**Source:** [DataDog/pup/SKILL.md](https://github.com/DataDog/pup/blob/652a6fd2f35428c719347715025a4e6168be4607/SKILL.md) · 893★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pup
description: Datadog API CLI with 49 command groups, 300+ subcommands. Skills and domain agents for monitoring, logs, APM, security, and infrastructure.
metadata:
  version: "0.25.0"
  author:
    name: Datadog
    email: support@datadoghq.com
  repository: https://github.com/DataDog/pup
  tags: datadog,cli,monitoring,logs,apm,metrics,security,infrastructure
---

# Datadog Pup CLI

Rust-based CLI for Datadog APIs. 49 command groups, 300+ subcommands across 53 command modules.

## Install Skills

```bash
# Install all skills and agents for the auto-detected AI assistant
pup skills install

# Or install for a specific platform (claude, cursor, codex, opencode, pi)
pup skills install claude
pup skills install codex
pup skills install cursor

# Install for every supported platform at once
pup skills install all

# Install a single skill by name
pup skills install claude --name dd-pup

# Default scope is user-global; pass --project to install into the repo
pup skills install claude --project

# List all available skills
pup skills list
```

## Skills

| Skill | Description |
|-------|-------------|
| **dd-pup** | Primary CLI - all pup commands, auth, site config |
| **dd-m
```

</details>
