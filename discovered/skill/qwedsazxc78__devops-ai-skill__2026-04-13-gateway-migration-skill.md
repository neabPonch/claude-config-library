---
name: qwedsazxc78__devops-ai-skill__2026-04-13-gateway-migration-skill
source: https://github.com/qwedsazxc78/devops-ai-skill/blob/a3959440f81307ef5135cdc0d59024de5fcd6d1b/docs/superpowers/plans/2026-04-13-gateway-migration-skill.md
repo: qwedsazxc78/devops-ai-skill
kind: skill
stars: 3
last_pushed: 2026-06-11T16:14:49Z
license: unknown
score: 9
domains: [devops, kubernetes, automation-agents, cloud-infrastructure]
tags: [skill-design, migration-pattern, agentic-workflows, k8s]
curated: 2026-06-16
curated_by: config-scout
---

# qwedsazxc78/devops-ai-skill — skill

**Why it's worth keeping:** It demonstrates the 'Thick Skill / Thin Pipeline' pattern and provides a rigorous testing strategy using input/expected fixtures, which is critical for verifying agentic reliability.

**Summary:** A highly sophisticated implementation plan for an autonomous DevOps skill that migrates NGINX Ingress to GKE Gateway API using a structured, multi-layered architecture.

**Source credibility:** High technical depth in documentation suggests professional-grade DevOps engineering.

**Recency:** Extremely current; focuses on modern GKE Gateway API standards and active development.

**Source:** [qwedsazxc78/devops-ai-skill/docs/superpowers/plans/2026-04-13-gateway-migration-skill.md](https://github.com/qwedsazxc78/devops-ai-skill/blob/a3959440f81307ef5135cdc0d59024de5fcd6d1b/docs/superpowers/plans/2026-04-13-gateway-migration-skill.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Gateway API Migration Skill Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Ship `*gateway-migrate`, a Zeus pipeline + `gateway-api-migration` skill that migrates NGINX master/minion Ingress topologies to GKE Gateway API resources with per-hostname DNS cutover, shipped as `devops-ai-skill` v1.7.0.

**Architecture:** One thick skill (`skills/gateway-api-migration/SKILL.md`) holds the authoritative logic; one thin pipeline (`prompts/zeus/gateway-migrate.md`) wraps it as an 8-step gate checklist. Reference material for the skill lives in `docs/gateway/` (canonical, human-facing) and is inline-copied to `skills/gateway-api-migration/references/`. The skill detects master/minion topology (primary) or standalone Ingress (fallback), emits a Gateway in a new `common.gateway/` module plus HTTPRoutes alongside existing minions in `common.service/`, and records progress in a resumable YAML state file.

**Tech Stack:** Bash shell scripting, Markdown (skill definitions), YAML (Kubernetes m
```

</details>
