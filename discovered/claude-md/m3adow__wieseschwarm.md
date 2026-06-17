---
name: m3adow__wieseschwarm
source: https://github.com/m3adow/wieseschwarm/blob/75f61b106567a24323e7d1604464a459a315d7b1/CLAUDE.md
repo: m3adow/wieseschwarm
kind: claude-md
stars: 2
last_pushed: 2026-06-15T19:56:45Z
license: agpl-3.0
score: 9
domains: [devops, kubernetes, gitops, security]
tags: [k8s, talos, sops, argocd, custom-agents]
curated: 2026-06-16
curated_by: config-scout
---

# m3adow/wieseschwarm — claude-md

**Why it's worth keeping:** It demonstrates advanced usage of Claude Code by cataloging specific custom skills/agents and provides strict YAML linting rules to prevent CI failures caused by AI edits.

**Summary:** Provides a highly structured guide for managing Kubernetes GitOps infrastructure, including encryption requirements and pre-commit stages. It serves as a central directory for project-specific custom Claude skills and agents.

**Source credibility:** High; the detail regarding Talos OS, SOPS encryption, and Kustomize patches indicates a real-world production DevOps environment.

**Recency:** Very current; explicitly leverages the latest Claude Code custom skills/agent patterns.

**Source:** [m3adow/wieseschwarm/CLAUDE.md](https://github.com/m3adow/wieseschwarm/blob/75f61b106567a24323e7d1604464a459a315d7b1/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository layout

- `kubernetes/` — active Kustomize manifests (ArgoCD GitOps); see `kubernetes/CLAUDE.md`
- `kubernetes/02_applications/apps/` — git submodule pointing to the private `wieseschwarm-applications` repo; contains user-facing application manifests
- `kubernetes_old/` — **deprecated** Flux-based structure; do not edit
- `talos/` — Talos OS patches; see `talos/CLAUDE.md`
- `.claude/` — Claude Code config (skills, agents, hooks, permissions)

The `wieseschwarm-applications` submodule is a **private** GitHub repository. It holds application manifests that must not be public (usernames, internal hostnames, etc.). After cloning this repo, populate the submodule with:

```bash
git submodule update --init
```

## Path conventions

Never use absolute paths in `.claude/` config files (settings.json, agent files, skills). Use paths relative to the repository root so the repo works regardless of where it is checked out.

## YAML conventions

All YAML documents must start with `---` (yamllint `document-start: required`).

Truthy-like values (`true`, `false`, `yes
```

</details>
