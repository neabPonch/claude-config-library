---
name: rohitg00__kubectl-mcp-server__skill
source: https://github.com/rohitg00/kubectl-mcp-server/blob/14f9c138a7efd80a2bbb83e7ecfcdbe259f6e598/kubernetes-skills/claude/k8s-helm/SKILL.md
repo: rohitg00/kubectl-mcp-server
kind: skill
stars: 909
last_pushed: 2026-04-08T22:37:48Z
license: mit
score: 9
domains: [devops, kubernetes, infrastructure, cli-tools]
tags: [helm, k8s, mcp, deployment]
curated: 2026-06-14
curated_by: config-scout
---

# rohitg00/kubectl-mcp-server — skill

**Why it's worth keeping:** The 'Priority Rules' table provides critical safety logic (e.g., templating before installing) and 'Common Workflows' offer proven multi-step execution paths for an agent to follow.

**Summary:** A highly structured operational playbook for managing Helm charts via MCP tools, emphasizing safe deployment practices.

**Source credibility:** High; the source is a CNCF Landscape project with significant community validation (900+ stars).

**Recency:** Current; utilizes modern agentic patterns of tool-calling heuristics and workflow orchestration.

**Source:** [rohitg00/kubectl-mcp-server/kubernetes-skills/claude/k8s-helm/SKILL.md](https://github.com/rohitg00/kubectl-mcp-server/blob/14f9c138a7efd80a2bbb83e7ecfcdbe259f6e598/kubernetes-skills/claude/k8s-helm/SKILL.md) · 909★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: k8s-helm
description: Manage Helm charts, releases, and repositories. Use for Helm installations, upgrades, rollbacks, chart development, and release management.
license: Apache-2.0
metadata:
  author: rohitg00
  version: "1.0.0"
  tools: 16
  category: workloads
---

# Helm Chart Management

Comprehensive Helm v3 operations using kubectl-mcp-server's 16 Helm tools.

## When to Apply

Use this skill when:
- User mentions: "helm", "chart", "release", "values", "repository"
- Operations: installing charts, upgrading releases, rollbacks
- Keywords: "package", "template", "lint", "repo add"

## Priority Rules

| Priority | Rule | Impact | Tools |
|----------|------|--------|-------|
| 1 | Template before install (dry run) | CRITICAL | `template_helm_chart` |
| 2 | Check existing releases first | CRITICAL | `list_helm_releases` |
| 3 | Lint charts before packaging | HIGH | `lint_helm_chart` |
| 4 | Note revision before upgrade | HIGH | `get_helm_history` |
| 5 | Verify values after upgrade | MEDIUM | `get_helm_values` |
| 6 | Update repos before search | LOW | `update_helm_repos` |

## Quick Reference

| Task | Tool | Example |
|------|------|---------|
| Install chart | `inst
```

</details>
