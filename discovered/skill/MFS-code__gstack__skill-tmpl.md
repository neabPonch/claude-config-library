---
name: MFS-code__gstack__skill-tmpl
source: https://github.com/MFS-code/gstack/blob/4e78d013baad718f7cdb8946556a2b4644265a71/retro/SKILL.md.tmpl
repo: MFS-code/gstack
kind: skill
stars: 6
last_pushed: 2026-03-24T16:48:36Z
license: mit
score: 9
domains: [cli-tools, devops, engineering-management]
tags: [git-analysis, retrospective, metrics]
curated: 2026-06-16
curated_by: config-scout
---

# MFS-code/gstack — skill

**Why it's worth keeping:** The precise midnight-aligned time window logic for Git commands and the multi-vector data gathering strategy (using specific `git log` formats to extract test ratios and session density) are elite techniques.

**Summary:** A high-level engineering retrospective skill that analyzes git history, contributor patterns, and code metrics to provide a 'team-aware' productivity report.

**Source credibility:** Strong; part of a specialized toolset (`gstack`) designed for high-output engineering workflows.

**Recency:** Very current; uses modern Git-based telemetry patterns ideal for Claude Code agents.

**Source:** [MFS-code/gstack/retro/SKILL.md.tmpl](https://github.com/MFS-code/gstack/blob/4e78d013baad718f7cdb8946556a2b4644265a71/retro/SKILL.md.tmpl) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: retro
preamble-tier: 2
version: 2.0.0
description: |
  Weekly engineering retrospective. Analyzes commit history, work patterns,
  and code quality metrics with persistent history and trend tracking.
  Team-aware: breaks down per-person contributions with praise and growth areas.
  Use when asked to "weekly retro", "what did we ship", or "engineering retrospective".
  Proactively suggest at the end of a work week or sprint.
allowed-tools:
  - Bash
  - Read
  - Write
  - Glob
  - AskUserQuestion
---

{{PREAMBLE}}

## Detect default branch

Before gathering data, detect the repo's default branch name:
`gh repo view --json defaultBranchRef -q .defaultBranchRef.name`

If this fails, fall back to `main`. Use the detected name wherever the instructions
say `origin/<default>` below.

---

# /retro — Weekly Engineering Retrospective

Generates a comprehensive engineering retrospective analyzing commit history, work patterns, and code quality metrics. Team-aware: identifies the user running the command, then analyzes every contributor with per-person praise and growth opportunities. Designed for a senior IC/CTO-level builder using Claude Code as a force multiplier.

## User-invoca
```

</details>
