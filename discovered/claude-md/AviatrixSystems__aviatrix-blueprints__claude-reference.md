---
name: AviatrixSystems__aviatrix-blueprints__claude-reference
source: https://github.com/AviatrixSystems/aviatrix-blueprints/blob/9aea6202cd97f99ef0bf933c1e0b2c2bbbdadb88/blueprints/aws-eks-multicluster/CLAUDE.md.reference
repo: AviatrixSystems/aviatrix-blueprints
kind: claude-md
stars: 8
last_pushed: 2026-06-15T19:32:16Z
license: apache-2.0
score: 9
domains: [infrastructure-as-code, devops, kubernetes, networking]
tags: [terraform, eks, aviatrix, multi-cluster]
curated: 2026-06-16
curated_by: config-scout
---

# AviatrixSystems/aviatrix-blueprints — claude-md

**Why it's worth keeping:** The use of an ASCII diagram to explain network connectivity and the explicit documentation of a multi-layer deployment sequence prevents AI from making order-of-operation errors.

**Summary:** Provides highly detailed architectural topology, dependency layers, and exact sequential commands for deploying complex Terraform infrastructure.

**Source credibility:** High quality; provided by Aviatrix, a major enterprise networking company.

**Recency:** Very recent (last pushed 0 months ago) and highly relevant to modern cloud infrastructure patterns.

**Source:** [AviatrixSystems/aviatrix-blueprints/blueprints/aws-eks-multicluster/CLAUDE.md.reference](https://github.com/AviatrixSystems/aviatrix-blueprints/blob/9aea6202cd97f99ef0bf933c1e0b2c2bbbdadb88/blueprints/aws-eks-multicluster/CLAUDE.md.reference) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a Terraform-based infrastructure repository for deploying an Aviatrix-managed multi-cluster Kubernetes demo environment, originally showcased at KubeCon EU 2024 to demonstrate Distributed Cloud Firewall (DCF) for Kubernetes capabilities.

## Architecture Overview

The infrastructure follows a **hub-and-spoke network topology** with **two EKS clusters**:

```
┌─────────────────────────────────────────┐
│   Aviatrix Transit Gateway (Hub)       │
│   Region: us-east-2                     │
│   CIDR: 10.2.0.0/20                     │
└────────┬───────────────────┬────────────┘
         │                   │
    ┌────▼─────┐      ┌─────▼──────┐
    │ Frontend │      │  Backend   │
    │  Spoke   │      │   Spoke    │
    │ 10.10/23 │      │  10.20/23  │
    │          │      │            │
    │ ┌──────┐ │      │ ┌────────┐ │
    │ │ EKS  │ │      │ │  EKS   │ │
    │ │Cluster│ │      │ │ Cluster│ │
    │ └──────┘ │      │ └────────┘ │
    └──────────┘      └────────────┘
         │                   │
         └─────────┬─────────┘
```

</details>
