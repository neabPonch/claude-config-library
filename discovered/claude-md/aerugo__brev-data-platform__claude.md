---
name: aerugo__brev-data-platform__claude
source: https://github.com/aerugo/brev-data-platform/blob/d821b33b2034ea33493b4cfb07f549be4cb78ea2/.CLAUDE.md
repo: aerugo/brev-data-platform
kind: claude-md
stars: 3
last_pushed: 2026-03-26T19:48:56Z
license: unknown
score: 9
domains: [infrastructure-as-code, data-platform, devops, ai-infra]
tags: [terraform, kubernetes, gitops, dagster, gpu]
curated: 2026-06-15
curated_by: config-scout
---

# aerugo/brev-data-platform — claude-md

**Why it's worth keeping:** Implements a sophisticated 'Planning Protocol' to force specification-first development and defines a hierarchy of specialized agents for different technical domains. The inclusion of critical deployment workflows (like the Dagster/submodule cycle) prevents common operational errors.

**Summary:** Provides comprehensive context for an IaC monorepo managing a GPU data platform via Kubernetes and GitOps. It outlines complex deployment cycles involving submodules and specialized toolchains.

**Source credibility:** Low star count but high density suggests a professional DevOps or Data Engineering context.

**Recency:** Highly current, utilizing modern AI-era technologies like NVIDIA NIM and advanced agentic patterns.

**Source:** [aerugo/brev-data-platform/.CLAUDE.md](https://github.com/aerugo/brev-data-platform/blob/d821b33b2034ea33493b4cfb07f549be4cb78ea2/.CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Brev Data Platform - Claude Code Instructions

## Project Overview

This is an Infrastructure as Code (IaC) monorepo that provisions an NVIDIA GPU server on Brev and deploys a complete data platform stack. The project serves as a **development environment** replicating an on-premises data platform setup to experiment with workflows using the NVIDIA Enterprise AI stack.

### End Goal

Deploy a fully functional data platform on-demand via GitOps that includes:
- **Data orchestration** with Dagster pipelines
- **Versioned data lake** with LakeFS + MinIO
- **Interactive notebooks** with Marimo
- **AI/ML inference** with NVIDIA NIM LLMs
- **Synthetic data generation** with NVIDIA Safe Synthesizer

All managed through ArgoCD GitOps, with infrastructure provisioned via Terraform.

## Tech Stack

| Layer | Technology | Purpose |
|-------|------------|---------|
| **Infrastructure** | Terraform | Provision NVIDIA Brev GPU instances |
| **Compute** | NVIDIA Brev | GPU cloud platform |
| **Kubernetes** | K3S | Lightweight single-node Kubernetes |
| **GitOps** | ArgoCD | Continuous deployment from Git |
| **CI/CD** | GitHub Actions | Build, test, and trigger deployments |
| **Storage** | Min
```

</details>
