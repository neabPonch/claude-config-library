---
name: fengshao1227__ccg-workflow__skill
source: https://github.com/fengshao1227/ccg-workflow/blob/84adbb0543b5a817319b493077299ceb9c76ba2a/templates/skills/domains/infrastructure/SKILL.md
repo: fengshao1227/ccg-workflow
kind: skill
stars: 5538
last_pushed: 2026-06-10T07:41:05Z
license: mit
score: 9
domains: [devops, infrastructure, cloud-native, kubernetes]
tags: [k8s, gitops, terraform, helm, iac]
curated: 2026-06-15
curated_by: config-scout
---

# fengshao1227/ccg-workflow — skill

**Why it's worth keeping:** Includes highly actionable 'Checklists' and 'Standard Structures' that allow an agent to validate user work against industry best practices rather than just syntax.

**Summary:** Provides a comprehensive mental model and operational standards for cloud-native infrastructure including Kubernetes, GitOps, and IaC.

**Source credibility:** High; source repository is well-starred and focuses on multi-model orchestration workflows.

**Recency:** Very recent/current with modern cloud-native standards.

**Source:** [fengshao1227/ccg-workflow/templates/skills/domains/infrastructure/SKILL.md](https://github.com/fengshao1227/ccg-workflow/blob/84adbb0543b5a817319b493077299ceb9c76ba2a/templates/skills/domains/infrastructure/SKILL.md) · 5538★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: infrastructure
description: 云原生基础设施。Kubernetes、Helm、Kustomize、Operator、CRD、GitOps、ArgoCD、Flux、IaC、Terraform、Pulumi、CDK。当用户提到 K8s、Helm、GitOps、IaC 时路由到此。
license: MIT
user-invocable: false
disable-model-invocation: false
---

# 云原生基础设施 · Infrastructure

## 域概览

```
                    GitOps 控制平面
                          |
        +-----------------+-----------------+
        |                 |                 |
    ArgoCD/Flux      Kubernetes         IaC 层
        |                 |                 |
   Git Repo ------> Helm/Kustomize --> Terraform/Pulumi
        |                 |                 |
    声明式配置        容器编排          云资源管理
```

---

## Kubernetes 容器编排

### Helm Chart 开发

标准结构：`Chart.yaml` + `values.yaml` + `templates/` + `charts/`

核心要点：
- Chart.yaml：`apiVersion: v2`, dependencies 声明子 Chart（condition 控制启用）
- values.yaml 设计：image / replicaCount / resources / autoscaling / service / ingress / probes / env / persistence
- Deployment 模板：使用 `_helpers.tpl` 定义 `fullname` / `labels` / `selectorLabels`
- 配置校验：`checksum/config: {{ include ... | sha256sum }}` 触发滚动更新
- 安全上下文：`runAsNonRoot: true, runAsUser: 1000`

关键命令：
- `helm lint` / `helm template --debug` 验证
- `hel
```

</details>
