---
name: Tyler-R-Kendrick__agent-skills__skill
source: https://github.com/Tyler-R-Kendrick/agent-skills/blob/b6b5c287c759ad66cf0d8788a9d956b5397bbe70/skills/iac/pulumi/SKILL.md
repo: Tyler-R-Kendrick/agent-skills
kind: skill
stars: 10
last_pushed: 2026-06-09T11:52:42Z
license: mit
score: 9
domains: [infrastructure, cloud-computing, iac]
tags: [pulumi, iac, typescript, python, aws]
curated: 2026-06-16
curated_by: config-scout
---

# Tyler-R-Kendrick/agent-skills — skill

**Why it's worth keeping:** It explicitly teaches the distinction between `.apply()` and `pulumi.interpolate`, a critical detail for preventing bugs in async output handling. The inclusion of 'ComponentResource' patterns provides a clear blueprint for modular IaC.

**Summary:** A high-quality Pulumi skill file providing language examples, CLI workflows, and specific technical nuances.

**Source credibility:** High quality personal repository with recent maintenance and highly structured content.

**Recency:** Very current; utilizes modern Pulumi idioms like interpolation over manual apply calls.

**Source:** [Tyler-R-Kendrick/agent-skills/skills/iac/pulumi/SKILL.md](https://github.com/Tyler-R-Kendrick/agent-skills/blob/b6b5c287c759ad66cf0d8788a9d956b5397bbe70/skills/iac/pulumi/SKILL.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pulumi
description: |
  Use when writing Pulumi programs for cloud infrastructure using TypeScript, Python, Go, or C#. Covers resource declarations, stacks, Outputs, component resources, and preview/up workflow.
  USE FOR: infrastructure in TypeScript/Python/Go/C#, imperative IaC, Pulumi stacks, component resources
  DO NOT USE FOR: declarative HCL-based IaC (use terraform), Azure-only Bicep DSL (use bicep), Kubernetes manifests (use kubernetes)
license: MIT
metadata:
  displayName: "Pulumi"
  author: "Tyler-R-Kendrick"
compatibility: claude, copilot, cursor
references:
  - title: "Pulumi Documentation"
    url: "https://www.pulumi.com/docs/"
  - title: "Pulumi GitHub Repository"
    url: "https://github.com/pulumi/pulumi"
  - title: "Pulumi Registry"
    url: "https://www.pulumi.com/registry/"
---

# Pulumi

## Overview
Pulumi is an open-source IaC platform that lets you define cloud infrastructure using general-purpose programming languages (TypeScript, Python, Go, C#, Java). Unlike HCL-based tools, you get full IDE support, loops, conditionals, type checking, and package management.

## TypeScript Example
```typescript
import * as aws from "@pulumi/aws";
import * as pu
```

</details>
