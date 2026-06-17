---
name: LukasNiessen__kubernetes-skill
source: https://github.com/LukasNiessen/kubernetes-skill/blob/dde723ab9f54aa4f9d8962cd85ffcb3ec8f36cc7/SKILL.md
repo: LukasNiessen/kubernetes-skill
kind: skill
stars: 238
last_pushed: 2026-06-04T22:17:43Z
license: mit
score: 9
domains: [devops, kubernetes, cloud-infrastructure, security]
tags: [k8s, helm, gitops, iac]
curated: 2026-06-15
curated_by: config-scout
---

# LukasNiessen/kubernetes-skill — skill

**Why it's worth keeping:** The 'Conditional Reference Retrieval' (CRR) pattern is highly transferable for complex domains, and the mandatory 'Capture execution context' phase ensures high-fidelity outputs based on cluster distribution and API versions.

**Summary:** A sophisticated diagnostic workflow that prevents Kubernetes hallucinations by enforcing structured context gathering and failure-mode analysis. It utilizes a tiered reference loading system to ensure platform-specific expertise is available without bloating the context window.

**Source credibility:** Strong; 238 stars and recent maintenance indicate a specialized, well-regarded toolset.

**Recency:** Very current; includes modern patterns like EKS Pod Identity and Karpenter.

**Source:** [LukasNiessen/kubernetes-skill/SKILL.md](https://github.com/LukasNiessen/kubernetes-skill/blob/dde723ab9f54aa4f9d8962cd85ffcb3ec8f36cc7/SKILL.md) · 238★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: kubernetes-skill
description: "Prevent Kubernetes hallucinations by diagnosing and fixing failure modes: insecure workload defaults, resource starvation, network exposure, privilege sprawl, fragile rollouts, and API drift. Use when generating, reviewing, refactoring, or migrating manifests, Helm charts, Kustomize overlays, cluster policies, and platform-specific Kubernetes work for EKS, GKE, AKS, OpenShift, GitOps controllers, or observability stacks."
---

# KubeShark: Failure-Mode Workflow for Kubernetes

Run this workflow top to bottom.

## 1) Capture execution context

Record before writing manifests:
- cluster version (e.g. 1.30, 1.31) and distribution (EKS, GKE, AKS, k3s, vanilla)
- target namespace and environment criticality (dev/staging/prod)
- workload type (Deployment, StatefulSet, Job, CronJob, DaemonSet)
- deployment method (raw YAML, Helm, Kustomize, operator-managed)
- policy enforcement (Pod Security Admission level, Kyverno, OPA/Gatekeeper)
- cloud provider and CNI (affects networking, storage classes, load balancers)
- platform controllers/add-ons (GitOps, observability, ingress, service mesh, autoscaling)

If unknown, state assumptions explicitly.

## 2
```

</details>
