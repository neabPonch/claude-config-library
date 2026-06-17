---
name: borghei__Claude-Skills__skill
source: https://github.com/borghei/Claude-Skills/blob/ce1405b1a55d1e98d9bda4ea23b987a56f71e93b/engineering/helm-chart-builder/SKILL.md
repo: borghei/Claude-Skills
kind: skill
stars: 271
last_pushed: 2026-06-15T18:22:21Z
license: other
score: 8
domains: [devops, kubernetes, infrastructure]
tags: [helm, k8s, cicd, validation]
curated: 2026-06-16
curated_by: config-scout
---

# borghei/Claude-Skills — skill

**Why it's worth keeping:** It includes explicit multi-step workflows and detailed 'Best Practices' tables that serve as a highly specific rubric for agentic reasoning.

**Summary:** Defines a structured protocol for analyzing, validating, and deploying Kubernetes Helm charts using specialized scripts.

**Source credibility:** High; the source repository is well-starred and contains deep, domain-specific expertise.

**Recency:** Extremely recent/future-dated metadata suggests it is current with modern toolchains.

**Source:** [borghei/Claude-Skills/engineering/helm-chart-builder/SKILL.md](https://github.com/borghei/Claude-Skills/blob/ce1405b1a55d1e98d9bda4ea23b987a56f71e93b/engineering/helm-chart-builder/SKILL.md) · 271★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: helm-chart-builder
description: >
  This skill should be used when the user asks to "analyze Helm charts",
  "validate Helm values", "review chart structure", "check Kubernetes Helm
  templates", or "audit chart dependencies and configuration".
license: MIT + Commons Clause
metadata:
  version: 1.0.0
  author: borghei
  category: engineering
  domain: kubernetes
  updated: 2026-04-02
  tags: [helm, kubernetes, k8s, charts, devops]
---
# Helm Chart Builder

> **Category:** Engineering
> **Domain:** Kubernetes & Helm

## Overview

The **Helm Chart Builder** skill provides automated analysis of Helm charts including structure validation, values checking, template inspection, and dependency review. It helps teams maintain high-quality charts with correct configurations, proper security contexts, and complete documentation.

## Quick Start

```bash
# Analyze chart structure and quality
python scripts/chart_analyzer.py --path ./charts/my-app

# Validate values.yaml against chart requirements
python scripts/values_validator.py --chart ./charts/my-app --values values-prod.yaml

# JSON output for CI
python scripts/chart_analyzer.py --path ./charts/my-app --format json

# Validate
```

</details>
