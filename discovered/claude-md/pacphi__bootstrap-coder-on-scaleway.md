---
name: pacphi__bootstrap-coder-on-scaleway
source: https://github.com/pacphi/bootstrap-coder-on-scaleway/blob/b13b8c3c4f4d6699617446908e54b22d4b709eba/CLAUDE.md
repo: pacphi/bootstrap-coder-on-scaleway
kind: claude-md
stars: 2
last_pushed: 2026-04-15T09:13:30Z
license: mit
score: 9
domains: [devops, infrastructure-as-code, kubernetes]
tags: [terraform, kubernetes, automation, iac]
curated: 2026-06-15
curated_by: config-scout
---

# pacphi/bootstrap-coder-on-scaleway — claude-md

**Why it's worth keeping:** The 'Two-Phase Troubleshooting' section is exceptional; it tells the AI exactly how to pivot from infrastructure failures to application troubleshooting. The inclusion of specific utility commands for remote state and cost management makes the agent highly actionable.

**Summary:** Defines a two-phase Terraform deployment strategy for Kubernetes-based development environments. It provides highly structured command sets for lifecycle management, cost analysis, and environment state.

**Source credibility:** High-quality specialized automation project with recent maintenance.

**Recency:** Very current, explicitly integrating Claude Code workflows.

**Source:** [pacphi/bootstrap-coder-on-scaleway/CLAUDE.md](https://github.com/pacphi/bootstrap-coder-on-scaleway/blob/b13b8c3c4f4d6699617446908e54b22d4b709eba/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **Terraform-based Infrastructure as Code (IaC)** project that deploys enterprise-grade **Coder development environments** on **Scaleway's managed Kubernetes** (Kapsule). The system provides 21+ workspace templates, multi-environment deployment, comprehensive cost management, and AI-enhanced development capabilities.

**Core Technology Stack:**

- **Infrastructure**: Terraform (≥1.13.3) with Scaleway provider
- **Container Platform**: Kubernetes on Scaleway Kapsule with Cilium CNI
- **Application**: Coder development platform with workspace templates
- **Database**: Managed PostgreSQL with environment-specific configurations
- **Orchestration**: Helm for application deployment
- **State Storage**: Remote state using Scaleway Object Storage (S3-compatible)

## Two-Phase Deployment Architecture

The system uses a **two-phase deployment architecture** that separates infrastructure provisioning from application deployment for enhanced reliability and troubleshooting capabilities:

**Phase 1: Infrastructure** (`environments/{env}/infra/`)

-
```

</details>
