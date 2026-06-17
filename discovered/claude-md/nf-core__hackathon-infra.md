---
name: nf-core__hackathon-infra
source: https://github.com/nf-core/hackathon-infra/blob/7258aa9c5c09970a12dcf1c2e0a71a46f3c21319/CLAUDE.md
repo: nf-core/hackathon-infra
kind: claude-md
stars: 2
last_pushed: 2026-03-10T20:11:09Z
license: mit
score: 9
domains: [infrastructure-as-code, devops, aws]
tags: [terraform, safety-guardrails, aws, operational-procedures]
curated: 2026-06-16
curated_by: config-scout
---

# nf-core/hackathon-infra — claude-md

**Why it's worth keeping:** The 'Critical Safety Rules' section explicitly forbids dangerous commands with detailed reasoning/incidents, and the AWS account context provides crucial scoping to prevent accidental resource destruction.

**Summary:** Provides rigorous safety guardrails and procedural skills for managing sensitive Terraform infrastructure.

**Source credibility:** nf-core is a highly respected bioinformatics community; documentation quality reflects this.

**Recency:** Very current; includes an incident report from 2026 (likely forward-dated or extremely recent).

**Source:** [nf-core/hackathon-infra/CLAUDE.md](https://github.com/nf-core/hackathon-infra/blob/7258aa9c5c09970a12dcf1c2e0a71a46f3c21319/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AI Agent Guidelines for Hackathon Terraform

Instructions for AI agents working on this Terraform infrastructure project.

## Project Overview

This repository deploys the nf-core hackathon virtual event infrastructure:
- **WorkAdventure** - Virtual office platform (app.hackathon.nf-co.re)
- **LiveKit** - WebRTC media server for proximity audio/video
- **Coturn** - TURN server for NAT traversal
- **Jitsi** - Video conferencing for meeting rooms

## Skills

Skills provide step-by-step procedures for common tasks. They load automatically based on user intent, or explicitly via `/deploy`, `/teardown`, `/debug`, `/maps`.

| Skill | When to Use |
|-------|-------------|
| `deploy` | Setting up for a new event, first-time deployment, recovering from destruction |
| `teardown` | Event is over, cleanup needed, starting fresh |
| `debug` | Services unhealthy, users report problems, OAuth/video/maps not working |
| `maps` | Working with map files, syncing changes, setting up interactive zones |

---

## CRITICAL: Terraform Safety Rules

### NEVER Do Without Explicit User Confirmation

| Operation | Risk |
|-----------|------|
| `terraform force-unlock` | Corrupts state if another process i
```

</details>
