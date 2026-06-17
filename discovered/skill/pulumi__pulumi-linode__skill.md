---
name: pulumi__pulumi-linode__skill
source: https://github.com/pulumi/pulumi-linode/blob/3b3b12a0dad47d87af69f6bb3b47a7106c56b8d7/.claude/skills/pulumi-upgrade-provider/SKILL.md
repo: pulumi/pulumi-linode
kind: skill
stars: 31
last_pushed: 2026-06-14T07:22:17Z
license: apache-2.0
score: 9
domains: [devops, infrastructure-as-code]
tags: [automation, workflow, pulumi, maintenance]
curated: 2026-06-15
curated_by: config-scout
---

# pulumi/pulumi-linode — skill

**Why it's worth keeping:** Implements rigorous 'Session Completion Requirements' and specific 'When to Stop' logic to prevent infinite loops or token waste. Uses high-quality technical guardrails against state confusion (e.g., banning `cd`) and handles long-running processes via timeouts.

**Summary:** Automates Pulumi provider upgrades by driving the `upgrade-provider` tool and iteratively resolving failure modes. It manages a complete lifecycle from installation to PR updates.

**Source credibility:** High; comes from a well-maintained, official Pulumi resource provider repository.

**Recency:** Current; uses modern patterns for agentic Git and CLI tool interaction.

**Source:** [pulumi/pulumi-linode/.claude/skills/pulumi-upgrade-provider/SKILL.md](https://github.com/pulumi/pulumi-linode/blob/3b3b12a0dad47d87af69f6bb3b47a7106c56b8d7/.claude/skills/pulumi-upgrade-provider/SKILL.md) · 31★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pulumi-upgrade-provider
description: Automate Pulumi provider repo upgrades with the `upgrade-provider` tool. Use when upgrading a pulumi provider repository to a new upstream version, running `upgrade-provider`, and addressing its common failure modes like patch conflicts or missing module mappings.
---

# Pulumi Upgrade Provider

## Prerequisites

First, install the `upgrade-provider` tool:

```bash
go install github.com/pulumi/upgrade-provider@latest
```

After installation, the tool will be in your PATH and you can run it directly as `upgrade-provider`.

**IMPORTANT:**
- Do NOT try to modify PATH or use absolute paths to run the tool
- Do NOT try to find where the tool was installed
- Just run `upgrade-provider` directly after installing - if it's not found (exit code 127), report this as an environment configuration issue and stop

## CRITICAL: Session Completion Requirements

**DO NOT end this session until one of these conditions is met:**

1. **Success**: The `upgrade-provider` command completes successfully AND you have retrieved the PR URL
2. **Explicit failure**: You have hit a stopping condition listed in "When to Stop and Report Failure" below

**You MUST NOT
```

</details>
