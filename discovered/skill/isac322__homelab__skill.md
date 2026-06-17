---
name: isac322__homelab__skill
source: https://github.com/isac322/homelab/blob/757dc492dc237d15201f8c5eb57ac40e6c8e9753/.claude/skills/homelab-version-checker/SKILL.md
repo: isac322/homelab
kind: skill
stars: 10
last_pushed: 2026-06-14T13:11:02Z
license: unknown
score: 9
domains: [devops, kubernetes, gitops, infrastructure-automation]
tags: [k8s, helm, argocd, version-management]
curated: 2026-06-15
curated_by: config-scout
---

# isac322/homelab — skill

**Why it's worth keeping:** It demonstrates a sophisticated 'Recall vs. Reflect' memory architecture and provides highly actionable logic for parsing nested configuration hierarchies.

**Summary:** An advanced GitOps auditor that scans ArgoCD manifests to discover workloads and checks upstream versions using specific CLI tools.

**Source credibility:** The source is a specialized homelab repo, but the engineering of the skill shows high technical density.

**Recency:** Highly current; integrates modern tools like skopeo/crane and advanced agentic memory patterns.

**Source:** [isac322/homelab/.claude/skills/homelab-version-checker/SKILL.md](https://github.com/isac322/homelab/blob/757dc492dc237d15201f8c5eb57ac40e6c8e9753/.claude/skills/homelab-version-checker/SKILL.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: homelab-version-checker
description: "Scan a GitOps repository to detect all deployed Kubernetes workloads (Helm charts, Kustomize, raw YAML, pinned container images), check upstream sources for version updates, and generate a detailed upgrade report with changelog summaries, breaking change analysis, and safety-level classifications (Safe / Config / External / Migration / Breaking). Then optionally execute upgrades with appropriate caution per safety level. Use this skill whenever the user mentions version updates, checking for outdated workloads, upgrade planning, dependency updates, or wants to know if anything in their cluster needs updating — even if they don't explicitly say 'version check'. Also trigger when the user asks about Helm chart updates, image tag bumps, or GitOps maintenance."
---

# Homelab Version Checker

Scan a GitOps repository managed by ArgoCD to build a complete inventory of deployed workloads, check upstream sources for version updates, analyze changelogs and breaking changes, classify upgrade safety, and produce a concise, actionable report. Then, on user request, execute upgrades with the right level of caution.

## Phase 0: Memory — Recall Pr
```

</details>
