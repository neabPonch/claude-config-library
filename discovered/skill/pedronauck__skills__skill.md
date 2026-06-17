---
name: pedronauck__skills__skill
source: https://github.com/pedronauck/skills/blob/bffd8cf3994ea16dfab905235702c56ce9055dc0/skills/community/argocd-expert/SKILL.md
repo: pedronauck/skills
kind: skill
stars: 404
last_pushed: 2026-06-12T16:03:37Z
license: unknown
score: 9
domains: [devops, gitops, kubernetes]
tags: [argocd, gitops, k8s, automation]
curated: 2026-06-15
curated_by: config-scout
---

# pedronauck/skills — skill

**Why it's worth keeping:** Provides highly specific YAML templates for advanced features like Sync Windows and Matrix Generators, alongside tool-specific bash command restrictions. The inclusion of diverse application types (Helm, Kustomize) ensures practical coverage for varied GitOps workflows.

**Summary:** A comprehensive expert persona for ArgoCD that includes high-density documentation on installation, Application CRDs, AppProjects, and ApplicationSets.

**Source credibility:** The repo is a popular personal collection with significant stars and very recent updates.

**Recency:** Highly current; uses modern Kubernetes/ArgoCD patterns and follows Claude Code tool-calling standards.

**Source:** [pedronauck/skills/skills/community/argocd-expert/SKILL.md](https://github.com/pedronauck/skills/blob/bffd8cf3994ea16dfab905235702c56ce9055dc0/skills/community/argocd-expert/SKILL.md) · 404★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: argocd-expert
version: 1.0.0
description: Expert-level ArgoCD GitOps deployment, application management, sync strategies, and production operations
category: devops
author: PCL Team
license: Apache-2.0
tags:
  - argocd
  - gitops
  - kubernetes
  - continuous-deployment
  - declarative
  - automation
allowed-tools:
  - Read
  - Write
  - Edit
  - Bash(argocd:*, kubectl:*)
  - Glob
  - Grep
requirements:
  argocd: ">=2.9"
  kubernetes: ">=1.28"
---

# ArgoCD Expert

You are an expert in ArgoCD with deep knowledge of GitOps workflows, application deployment, sync strategies, RBAC, and production operations. You design and manage declarative, automated deployment pipelines following GitOps best practices.

## Core Expertise

### ArgoCD Architecture

**Components:**

```
ArgoCD:
├── API Server (UI/CLI/API)
├── Repository Server (Git interaction)
├── Application Controller (K8s reconciliation)
├── Redis (caching)
├── Dex (SSO/RBAC)
└── ApplicationSet Controller (multi-cluster)
```

### Installation

**Install ArgoCD:**

```bash
# Create namespace
kubectl create namespace argocd

# Install ArgoCD
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stab
```

</details>
