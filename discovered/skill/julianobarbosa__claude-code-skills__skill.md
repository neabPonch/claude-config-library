---
name: julianobarbosa__claude-code-skills__skill
source: https://github.com/julianobarbosa/claude-code-skills/blob/758c93f6ea4b826dd8c884f2c205fe4aafedbfb5/skills/argocd/SKILL.md
repo: julianobarbosa/claude-code-skills
kind: skill
stars: 79
last_pushed: 2026-06-11T19:21:44Z
license: mit
score: 9
domains: [devops, gitops, cli-tools, infrastructure]
tags: [argocd, kubernetes, automation, gitops]
curated: 2026-06-15
curated_by: config-scout
---

# julianobarbosa/claude-code-skills — skill

**Why it's worth keeping:** Provides exact curl command structures with full JSON payloads and detailed YAML specs, which is crucial for preventing agent hallucinations during complex GitOps automation.

**Summary:** A highly actionable skill file for ArgoCD that bridges the gap between CLI commands and raw REST API interactions.

**Source credibility:** High-density technical content; source shows very recent updates.

**Recency:** Current; follows modern ArgoCD CLI and API standards.

**Source:** [julianobarbosa/claude-code-skills/skills/argocd/SKILL.md](https://github.com/julianobarbosa/claude-code-skills/blob/758c93f6ea4b826dd8c884f2c205fe4aafedbfb5/skills/argocd/SKILL.md) · 79★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: argocd
description: Complete ArgoCD CLI and REST API skill for GitOps automation. Use when working with ArgoCD for: (1) Managing Applications - create, sync, delete, rollback, get status, wait for health, view logs, (2) ApplicationSets - templated multi-cluster deployments with generators, (3) Projects - RBAC, source/destination restrictions, sync windows, roles, (4) Repositories - add/remove Git repos, Helm charts, OCI registries, credential templates, (5) Clusters - register, rotate credentials, manage multi-cluster, (6) Accounts - generate tokens, manage users, check permissions, (7) Admin operations - export/import, settings validation, RBAC testing, notifications, (8) Troubleshooting - sync issues, health problems, connection errors. Supports both REST API (curl/HTTP) and CLI approaches with bearer token authentication.
---

# ArgoCD Skill

Complete ArgoCD operations via REST API and CLI with bearer token authentication.

## Authentication Setup

Generate and use bearer tokens for all operations:

```bash
# Generate token (requires existing login)
argocd login $ARGOCD_SERVER --username admin --password $ARGOCD_PASSWORD
ARGOCD_TOKEN=$(argocd account generate-token)

#
```

</details>
