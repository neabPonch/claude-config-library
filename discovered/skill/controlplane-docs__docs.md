---
name: controlplane-docs__docs
source: https://github.com/controlplane-docs/docs/blob/f3b7d968e5b797a8b4394bad3cd0a2343f9ef91c/skill.md
repo: controlplane-docs/docs
kind: skill
stars: 2
last_pushed: 2026-06-14T05:36:55Z
license: unknown
score: 9
domains: [infrastructure, devops, cli-tools]
tags: [multi-cloud, containerization, mcp, guardrails]
curated: 2026-06-14
curated_by: config-scout
---

# controlplane-docs/docs — skill

**Why it's worth keeping:** The 'Guardrails' section provides exceptional, high-stakes instructions—such as mandatory identity/policy/reference chains for secrets and required context confirmation—that prevent common agent errors and silent failures.

**Summary:** Defines a highly structured operational skill for managing multi-cloud containerized workloads via the `cpln` CLI.

**Source credibility:** High; official documentation from Control Plane Corporation.

**Recency:** Current; explicitly mentions Claude Code and MCP Server integrations.

**Source:** [controlplane-docs/docs/skill.md](https://github.com/controlplane-docs/docs/blob/f3b7d968e5b797a8b4394bad3cd0a2343f9ef91c/skill.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cpln
description: Use when deploying and managing containerized workloads across multiple clouds (AWS, GCP, Azure, private), configuring multi-cloud infrastructure, managing secrets and access control, setting up identities for credential-free cloud access, automating deployments with GitOps, or connecting AI tools to Control Plane via the AI Plugin or MCP Server.
license: Apache-2.0
compatibility: Requires cpln CLI (npm @controlplane/cli, Homebrew, or binary), AI Plugin (Claude Code, Codex, Gemini CLI — bundles the MCP Server), or MCP Server (https://mcp.cpln.io/mcp). Works with any CI/CD platform, Terraform, Pulumi, and Kubernetes.
allowed-tools: cpln
metadata:
  mintlify-proj: controlplanecorporation
  author: controlplane
  version: '3.0'
---

# Control Plane Skill

## What is Control Plane

Control Plane is a hybrid platform for deploying and managing containerized workloads across AWS, GCP, Azure, and private clouds from a unified interface. It abstracts cloud provider differences behind a consistent API, CLI (`cpln`), Console UI, Terraform provider, Pulumi provider, Kubernetes Operator, and MCP Server. Certified PCI DSS Level 1, SOC 2 Type II, and HIPAA-eligible.
```

</details>
