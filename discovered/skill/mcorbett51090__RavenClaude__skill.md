---
name: mcorbett51090__RavenClaude__skill
source: https://github.com/mcorbett51090/RavenClaude/blob/1feb6d35dd37968f81758f90e2d24f864bd7db31/plugins/azure-cloud/skills/compute-host-selection/SKILL.md
repo: mcorbett51090/RavenClaude
kind: skill
stars: 3
last_pushed: 2026-06-16T07:24:07Z
license: other
score: 8
domains: [cloud-infrastructure, azure, devops, architecture]
tags: [azure, compute, decision-tree, iaac]
curated: 2026-06-17
curated_by: config-scout
---

# mcorbett51090/RavenClaude — skill

**Why it's worth keeping:** Uses logical decision trees and comparison tables to minimize ambiguity; provides specific technical implementation details like Bicep snippets and SKU-tier recommendations.

**Summary:** A highly structured decision playbook that guides an AI through choosing the optimal Azure compute service based on specific workload criteria.

**Source credibility:** The content quality is high and demonstrates professional architectural expertise despite the relatively low star count.

**Recency:** Very current, referencing 2024 Bicep resource versions and modern Azure service patterns.

**Source:** [mcorbett51090/RavenClaude/plugins/azure-cloud/skills/compute-host-selection/SKILL.md](https://github.com/mcorbett51090/RavenClaude/blob/1feb6d35dd37968f81758f90e2d24f864bd7db31/plugins/azure-cloud/skills/compute-host-selection/SKILL.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: compute-host-selection
description: "Decision playbook for choosing the right Azure compute service — App Service, Container Apps, Azure Functions, Static Web Apps, or AKS — based on workload shape, ops burden, and scaling requirements."
---

# Compute Host Selection

## When to Use This Skill

Use when a new workload needs a home on Azure and the right compute service is not obvious, or when reviewing an existing workload that may be over- or under-engineered for its current host.

## 1. The Primary Decision Tree

Answer these questions in order:

| Question | If YES | If NO |
|---|---|---|
| Is it purely static (HTML/JS/CSS + optional serverless API)? | **Static Web Apps** | Continue |
| Is it event-driven, short-duration (< 10 min), and triggered by a queue/timer/HTTP? | **Azure Functions** | Continue |
| Does it need HTTP scaling to zero AND you want container-native packaging? | **Container Apps** | Continue |
| Does it need the full Kubernetes API (CRDs, operators, custom schedulers)? | **AKS** | Continue |
| Everything else (traditional web app, always-on API, background service) | **App Service** | — |

## 2. Service Comparison Table

| Service | Scale-to-zero | C
```

</details>
