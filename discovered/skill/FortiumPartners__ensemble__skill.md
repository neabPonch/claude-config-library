---
name: FortiumPartners__ensemble__skill
source: https://github.com/FortiumPartners/ensemble/blob/d8d52e824e6c35508c599b107a7728e73d56f405/packages/pi/skills/flyio/SKILL.md
repo: FortiumPartners/ensemble
kind: skill
stars: 10
last_pushed: 2026-06-09T18:02:45Z
license: mit
score: 9
domains: [devops, infrastructure, deployment]
tags: [flyio, paas, docker, templates]
curated: 2026-06-15
curated_by: config-scout
---

# FortiumPartners/ensemble — skill

**Why it's worth keeping:** Includes critical 'When to use' vs 'When NOT to use' architectural guidance and provides complete configuration pairs (orchestration + containerization) rather than just snippets.

**Summary:** Provides specialized deployment templates for Fly.io across multiple runtimes, including both fly.toml and Dockerfile configurations.

**Source credibility:** High-quality modular structure from a focused ecosystem repository.

**Recency:** Current; aligns with modern PaaS deployment patterns.

**Source:** [FortiumPartners/ensemble/packages/pi/skills/flyio/SKILL.md](https://github.com/FortiumPartners/ensemble/blob/d8d52e824e6c35508c599b107a7728e73d56f405/packages/pi/skills/flyio/SKILL.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: flyio
description: '1. [fly.toml Quick Reference](#flytoml-quick-reference)'
---
# Fly.io Infrastructure Skills

**Version**: 1.0.0 | **Target Size**: <25KB | **Purpose**: Fast reference for Fly.io deployments and global application distribution

---

## Overview

**What is Fly.io**: Modern platform-as-a-service (PaaS) for deploying applications globally with minimal configuration. Fly.io transforms containers into micro-VMs that run on physical hardware across 30+ regions worldwide.

**When to Use Fly.io**:
- Simple to moderate applications requiring global distribution
- Fast deployments without complex Kubernetes orchestration
- Minimal operations overhead with PaaS simplicity
- Edge computing and low-latency requirements (anycast routing)
- Startup/SaaS applications with unpredictable traffic patterns
- Databases requiring multi-region active replication (Fly Postgres)

**When to Use Kubernetes Instead**:
- Complex microservices architectures with 10+ interdependent services
- Existing Kubernetes expertise and tooling investment
- Hybrid cloud or multi-cloud requirements (cloud-agnostic)
- Advanced orchestration needs (service mesh, custom operators, advanced scheduli
```

</details>
