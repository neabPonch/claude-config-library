---
name: OpenRouterLabs__spawn__skill
source: https://github.com/OpenRouterLabs/spawn/blob/fe137e426e5096f0abb2de6fc5c70f609bd61308/.claude/skills/update-team/SKILL.md
repo: OpenRouterLabs/spawn
kind: skill
stars: 193
last_pushed: 2026-06-06T05:11:05Z
license: apache-2.0
score: 8
domains: [devops, agents-ai, system-administration]
tags: [orchestration, reconciliation-loop, service-management]
curated: 2026-06-15
curated_by: config-scout
---

# OpenRouterLabs/spawn — skill

**Why it's worth keeping:** Implements a high-integrity reconciliation loop: reading a source of truth, verifying compliance via grep/test, patching state with sed, and validating health via curl.

**Summary:** An orchestration skill that synchronizes agent services by reconciling wrapper scripts and systemd units against a central configuration.

**Source credibility:** High; OpenRouterLabs is an active organization with frequently updated repositories.

**Recency:** Current; utilizes modern systemd and shell workflows standard for agentic CLI environments.

**Source:** [OpenRouterLabs/spawn/.claude/skills/update-team/SKILL.md](https://github.com/OpenRouterLabs/spawn/blob/fe137e426e5096f0abb2de6fc5c70f609bd61308/.claude/skills/update-team/SKILL.md) · 193★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: update-team
description: Update agent team services with latest configuration from setup-agent-team and restart them
argument-hint: "[service-name] [--check-only]"
allowed-tools: Bash, Read, Edit, Glob, Grep
---

# Update Agent Team Services

Update the trigger server and wrapper scripts with the latest configuration from `.claude/skills/setup-agent-team/SKILL.md`, then restart the services to apply changes.

## Arguments

- `service-name` (optional) — Update only this service (e.g., `discovery`, `refactor`, `security`, `qa`). If omitted, updates all services.
- `--check-only` — Show what would be updated without making changes or restarting services.

**$ARGUMENTS**

## Overview

This skill:
1. Reads the latest setup-agent-team SKILL.md for current best practices
2. Identifies all deployed services by scanning for `start-*.sh` wrappers
3. Updates wrapper scripts with correct env vars and paths
4. Restarts systemd services to apply changes
5. Verifies services are running and healthy

## Step 1: Determine repository path

Detect the current repository path:

```bash
REPO_ROOT="$(cd /root/spawn 2>/dev/null && pwd || cd /home/sprite/spawn 2>/dev/null && pwd)"
echo "Reposito
```

</details>
