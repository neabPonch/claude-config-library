---
name: kubesphere__kubesphere__skill
source: https://github.com/kubesphere/kubesphere/blob/620af71dc080eb37f76e6d231d33ec85a337cd18/skills/kubesphere-devops-argocd/SKILL.md
repo: kubesphere/kubesphere
kind: skill
stars: 16968
last_pushed: 2026-06-04T06:32:03Z
license: other
score: 9
domains: [devops, kubernetes, gitops]
tags: [argocd, kubesphere, gitops, multi-tenancy]
curated: 2026-06-16
curated_by: config-scout
---

# kubesphere/kubesphere — skill

**Why it's worth keeping:** Includes highly specific curl templates for API-driven resource creation and clear architectural diagrams explaining cross-namespace controllers.

**Summary:** Provides technical context for managing GitOps via KubeSphere's customized ArgoCD implementation, distinguishing between admin and tenant workflows.

**Source credibility:** High; KubeSphere is a major enterprise Kubernetes platform with significant community traction.

**Recency:** 

**Source:** [kubesphere/kubesphere/skills/kubesphere-devops-argocd/SKILL.md](https://github.com/kubesphere/kubesphere/blob/620af71dc080eb37f76e6d231d33ec85a337cd18/skills/kubesphere-devops-argocd/SKILL.md) · 16968★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: kubesphere-devops-argocd
description: Use when configuring ArgoCD in KubeSphere DevOps, including GitOps deployments, application management, SSO setup, or troubleshooting ArgoCD issues
---

# KubeSphere DevOps ArgoCD Configuration

## Overview

KubeSphere DevOps includes **ArgoCD v2.11.7** as a bundled subchart for GitOps continuous deployment. ArgoCD follows the declarative GitOps pattern, automatically syncing application state with Git repositories.

## When to Use

- Setting up GitOps continuous deployment
- Configuring ArgoCD applications and ApplicationSets
- Enabling SSO authentication via Dex
- Managing multi-cluster deployments
- Troubleshooting ArgoCD sync issues
- Configuring repository credentials

## KubeSphere GitOps Integration

### Two Ways to Create Applications

**1. Direct ArgoCD Application (Admin Only)**
- Created in `argocd` namespace
- Requires access to ArgoCD namespace
- Full control over ArgoCD configuration

**2. KubeSphere GitOps Application (Tenant-Friendly)**
- Created via `/kapis/gitops.kubesphere.io/v1alpha1/`
- Application CR created in tenant namespace
- KubeSphere automatically creates corresponding ArgoCD Application
- Tenant doesn't n
```

</details>
