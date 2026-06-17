---
name: stacksjs__stacks__skill
source: https://github.com/stacksjs/stacks/blob/f45503038424bce151f090ecec1ae88434f5ed56/.claude/skills/stacks-deploy/SKILL.md
repo: stacksjs/stacks
kind: skill
stars: 620
last_pushed: 2026-06-15T05:50:36Z
license: mit
score: 8
domains: [devops, deployment, fullstack-framework, cli-tools]
tags: [aws, typescript, infrastructure-as-code, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# stacksjs/stacks — skill

**Why it's worth keeping:** The inclusion of 'Gotchas' prevents common deployment failures, and the documentation of deploy hooks allows an agent to autonomously manage side effects like smoke tests or cache warming.

**Summary:** Provides a highly specific operational manual for deploying Stacks applications using its custom 'buddy' CLI. It outlines architectural modes, prerequisites, and lifecycle hooks.

**Source credibility:** High; comes from a modern, active full-stack framework repository with consistent maintenance.

**Recency:** Current; utilizes modern toolchains like Bun >= 1.3.0.

**Source:** [stacksjs/stacks/.claude/skills/stacks-deploy/SKILL.md](https://github.com/stacksjs/stacks/blob/f45503038424bce151f090ecec1ae88434f5ed56/.claude/skills/stacks-deploy/SKILL.md) · 620★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: stacks-deploy
description: Use when deploying a Stacks application — the deployment workflow (build → deploy), pre/post deploy hooks, server vs serverless mode selection, first-time deployment setup, deployment troubleshooting, or the buddy deploy command. For cloud infrastructure details (EC2, Lambda, CloudFormation, Route53, IAM), see stacks-cloud.
license: MIT
compatibility: Bun >= 1.3.0, TypeScript, AWS
allowed-tools: Read Edit Write Bash Grep Glob
---

# Stacks Deployment

The deployment workflow for Stacks applications.

## Quick Deploy

```bash
buddy deploy
```

## Deployment Prerequisites

1. **AWS credentials configured**: `buddy configure:aws`
2. **APP_KEY generated**: `buddy key:generate` (must be colon-separated format)
3. **APP_URL set** in `.env`
4. **Team configured** in `config/team.ts`

## Deployment Flow

1. **Validation** — checks APP_KEY format, AWS region, app URL, team config
2. **Build** — compiles application for production
3. **Infrastructure** — generates CloudFormation template via ts-cloud
4. **Deploy** — creates or updates the CloudFormation stack
   - Capabilities: CAPABILITY_IAM, CAPABILITY_NAMED_IAM
   - OnFailure: ROLLBACK
   - Tags: Envir
```

</details>
