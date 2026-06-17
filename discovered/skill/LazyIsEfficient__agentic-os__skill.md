---
name: LazyIsEfficient__agentic-os__skill
source: https://github.com/LazyIsEfficient/agentic-os/blob/ca5adfe833ef42e627a61660fb0839c3d857189f/.claude/skills/devops-engineer/SKILL.md
repo: LazyIsEfficient/agentic-os
kind: skill
stars: 11
last_pushed: 2026-06-12T18:35:17Z
license: mit
score: 9
domains: [devops, kubernetes, infrastructure-as-code]
tags: [k8s, pulumi, helm, safety-first, platform-engineering]
curated: 2026-06-16
curated_by: config-scout
---

# LazyIsEfficient/agentic-os — skill

**Why it's worth keeping:** The 'read actual state before proposing' rule directly mitigates LLM hallucination risks in infrastructure. It also provides excellent scope boundaries via its 'Not when' section to prevent agent drift.

**Summary:** A rigorous operational persona for Kubernetes and IaC management that enforces strict safety protocols through mandatory dry-runs and state verification.

**Source credibility:** High quality content suggesting experienced platform/SRE authorship, despite the modest star count.

**Recency:** Very current; focuses on modern toolchains like Pulumi and Kubernetes-centric workflows.

**Source:** [LazyIsEfficient/agentic-os/.claude/skills/devops-engineer/SKILL.md](https://github.com/LazyIsEfficient/agentic-os/blob/ca5adfe833ef42e627a61660fb0839c3d857189f/.claude/skills/devops-engineer/SKILL.md) · 11★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: devops-engineer
description: Use when authoring or modifying infrastructure as code, working with Kubernetes (k8s, kubectl, cluster, namespace, RBAC, rollout, deployment), Helm (helm chart, helm upgrade, helm diff), Pulumi (pulumi stack, pulumi up, pulumi preview, IaC), or CI/CD pipeline DevOps mechanics (build systems, artifact publishing, environment promotion). Triggers on terms like "DevOps", "platform engineering", "cluster admin", "network policy", "resource quota", "pod spec", or "kubeconfig". For SRE/on-call/incident response see site-reliability-engineering. For Solidity/EVM contracts see web3-smart-contract-engineering. Not for GitHub Actions YAML authoring — use deployment-pipelines.
when_to_use: |
  Use when: authoring or reviewing Pulumi stacks or other IaC, Kubernetes Day-2
  operations (deployments, rollouts, namespace admin, RBAC, resource quotas,
  network policies), Helm chart authoring or upgrading, CI/CD pipeline DevOps
  mechanics (build configs, artifact registries, environment promotion gates),
  cluster administration, or any infrastructure-as-code change that needs
  preview/diff/apply discipline.

  Not when: configuring a service mesh (Istio, Li
```

</details>
