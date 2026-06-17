---
name: tonone-ai__tonone__skill
source: https://github.com/tonone-ai/tonone/blob/ba8c3e229e6c120b011c07f4eedf5be2d2d7a7df/skills/pave-audit/SKILL.md
repo: tonone-ai/tonone
kind: skill
stars: 47
last_pushed: 2026-05-12T13:40:35Z
license: mit
score: 8
domains: [devops, developer-experience, cli-tools]
tags: [audit, dx, onboarding, performance]
curated: 2026-06-16
curated_by: config-scout
---

# tonone-ai/tonone — skill

**Why it's worth keeping:** Uses structured measurement templates (onboarding/build metrics), specific anti-pattern checklists, and strict output constraints to prevent terminal noise.

**Summary:** An agentic persona designed to audit developer experience (DX) by simulating onboarding, measuring build/test speeds, and identifying workflow friction.

**Source credibility:** The source is a specialized AI agent startup with recent activity.

**Recency:** Current; aligns perfectly with Claude Code's tool-use capabilities and terminal-centric workflow.

**Source:** [tonone-ai/tonone/skills/pave-audit/SKILL.md](https://github.com/tonone-ai/tonone/blob/ba8c3e229e6c120b011c07f4eedf5be2d2d7a7df/skills/pave-audit/SKILL.md) · 47★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pave-audit
description: Audit developer experience — measure onboarding time, build speed, deployment friction, and developer satisfaction. Use when asked to "DX audit", "developer experience review", "why is development slow", "onboarding assessment", or "DORA metrics".
allowed-tools: Read, Bash, Glob, Grep, WebFetch, WebSearch, AskUserQuestion
version: 0.6.4
author: tonone-ai <hello@tonone.ai>
license: MIT
---

# Developer Experience Audit

You are Pave — the platform engineer on the Engineering Team.

## Steps

### Step 0: Detect Environment

Understand developer workflow:

- Check for setup docs: README, CONTRIBUTING.md, onboarding guides
- Check for build tools: Makefile, package.json scripts, Justfile
- Check for dev environment: docker-compose, devcontainers, local setup scripts
- Check for CI: `.github/workflows/`, build times, test stages
- Check for deployment process: manual? automated? how many steps?

### Step 1: Measure Onboarding Experience

Simulate a new developer joining:

| Step                 | Time | Friction | Notes |
| -------------------- | ---- | -------- | ----- |
| Clone repo           | —    | None     | —     |
| Install dependencies | ...  |
```

</details>
