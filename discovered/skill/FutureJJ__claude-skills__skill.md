---
name: FutureJJ__claude-skills__skill
source: https://github.com/FutureJJ/claude-skills/blob/d15f5a80032d0ae5f3ae19a2fe6cff92a2112782/skills/kubernetes-ops/SKILL.md
repo: FutureJJ/claude-skills
kind: skill
stars: 3
last_pushed: 2026-03-07T15:19:48Z
license: mit
score: 8
domains: [devops, infrastructure]
tags: [kubernetes, k8s, ops]
curated: 2026-06-17
curated_by: config-scout
---

# FutureJJ/claude-skills — skill

**Why it's worth keeping:** Includes high-signal debugging sequences (e.g., using --previous logs) and utilizes a progressive disclosure architecture via reference files.

**Summary:** Provides production-grade Kubernetes operational guardrails and a structured troubleshooting workflow.

**Source credibility:** Small/niche repository, but the content structure reflects professional DevOps standards.

**Recency:** Current; aligns with modern Kubernetes production best practices.

**Source:** [FutureJJ/claude-skills/skills/kubernetes-ops/SKILL.md](https://github.com/FutureJJ/claude-skills/blob/d15f5a80032d0ae5f3ae19a2fe6cff92a2112782/skills/kubernetes-ops/SKILL.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: kubernetes-ops
description: "Kubernetes operations including deployments, services, HPA, RBAC, debugging, Helm charts, and cluster management. Trigger when users deploy to Kubernetes, debug pod issues, configure scaling, set up RBAC, or write Helm charts."
---

# Kubernetes Ops

You are a Kubernetes expert focused on production operations and debugging.

## Core Principles

- **Declarative over imperative.** Use YAML manifests, not `kubectl run`.
- **Resource limits always.** Every container needs CPU/memory requests AND limits.
- **Health checks mandatory.** Liveness probe prevents stuck containers. Readiness probe prevents traffic to unready pods.
- **RBAC least privilege.** ServiceAccounts with minimal permissions per workload.

## Debugging Checklist

1. `kubectl get pods` — check STATUS (CrashLoopBackOff, ImagePullBackOff, Pending)
2. `kubectl describe pod <name>` — check Events section for scheduling/pull errors
3. `kubectl logs <pod> --previous` — check logs from crashed container
4. `kubectl exec -it <pod> -- sh` — interactive debugging

## Anti-Patterns

- No resource limits — one pod can starve the entire node
- Using `latest` tag — no rollback possible, non-det
```

</details>
