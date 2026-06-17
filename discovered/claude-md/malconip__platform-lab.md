---
name: malconip__platform-lab
source: https://github.com/malconip/platform-lab/blob/0f4ab364d4e21df6356701c34eb395c7df13ea0b/claude.md
repo: malconip/platform-lab
kind: claude-md
stars: 0
last_pushed: 2026-01-29T18:57:29Z
license: unknown
score: 8
domains: [devops, kubernetes, gitops]
tags: [platform-engineering, k8s, argocd, crossplane]
curated: 2026-06-16
curated_by: config-scout
---

# malconip/platform-lab — claude-md

**Why it's worth keeping:** The 'Component Types' and 'Adding New Components' sections provide explicit decision trees (Option 1, 2, or 3) that prevent the LLM from deviating from established infrastructure patterns.

**Summary:** Provides a high-level architectural map and specific procedural patterns for extending a GitOps-driven Kubernetes platform.

**Source credibility:** Specialized technical demo repository with high-density domain expertise.

**Recency:** 

**Source:** [malconip/platform-lab/claude.md](https://github.com/malconip/platform-lab/blob/0f4ab364d4e21df6356701c34eb395c7df13ea0b/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Platform Lab - Claude Context Specification

## Overview

Local Kubernetes platform demonstrating GitOps, Platform Engineering, and Developer Experience patterns. Runs on Docker Desktop Kubernetes.

**Key Technologies:** ArgoCD (GitOps), Crossplane (Infrastructure as Code), Backstage (IDP), Gateway API (routing), kube-prometheus-stack (observability)

---

## Architecture

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                              GITOPS FLOW                                     │
│                                                                              │
│   bootstrap/install.sh                                                       │
│         │                                                                    │
│         ▼                                                                    │
│   ┌─────────────┐    watches    ┌────────────────────┐                       │
│   │ root-app    │──────────────▶│ platform/apps/     │                       │
│   │ (ArgoCD)    │               │ platform-apps.yaml │                       │
│   └─────────────┘               └────────────────────┘                       │
│
```

</details>
