---
name: J-Tech-Japan__Sekiban__iac-aws-claude
source: https://github.com/J-Tech-Japan/Sekiban/blob/d1cfd8a5e57887246a39a77961e2ad2b2ae5c8c5/tasks/876/infra/iac-aws-claude.md
repo: J-Tech-Japan/Sekiban
kind: claude-md
stars: 335
last_pushed: 2026-05-27T15:08:38Z
license: other
score: 8
domains: [infrastructure, devops, backend]
tags: [aws, cdk, iac, orleans]
curated: 2026-06-16
curated_by: config-scout
---

# J-Tech-Japan/Sekiban — claude-md

**Why it's worth keeping:** The explicit mapping of configuration schemas (JSON) and the modular construct-based approach provide perfect structure for AI to follow when modifying infrastructure.

**Summary:** Provides a rigorous blueprint for deploying an Orleans-based system on AWS using C# and CDK. It defines clear environment parity via JSON configuration and strict directory hierarchies.

**Source credibility:** High; sourced from a popular (335 stars) C# event-sourcing framework with recent maintenance.

**Recency:** Current; updated within the last month.

**Source:** [J-Tech-Japan/Sekiban/tasks/876/infra/iac-aws-claude.md](https://github.com/J-Tech-Japan/Sekiban/blob/d1cfd8a5e57887246a39a77961e2ad2b2ae5c8c5/tasks/876/infra/iac-aws-claude.md) · 335★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AWS Infrastructure as Code Design for Sekiban DCB + Orleans

## Overview

This document defines the IaC approach for deploying Sekiban DCB + Orleans on AWS, matching the Azure Bicep structure used in the Kenbai project.

### Goals
1. **Local deployment**: Deploy from developer machines using CLI
2. **CLI + IaC**: Infrastructure defined as code, deployed via AWS CLI/SDK
3. **GitHub Actions**: Automated CI/CD pipeline for continuous deployment
4. **Environment parity**: Support dev/stg/prod environments with parameterization

---

## IaC Tool Comparison

| Feature | AWS CDK (C#) | Terraform | CloudFormation |
|---------|-------------|-----------|----------------|
| Language | C#, TypeScript, Python | HCL | YAML/JSON |
| .NET Affinity | ✅ Excellent | ⚠️ Separate | ⚠️ Separate |
| Module Reuse | ✅ Constructs | ✅ Modules | ⚠️ Nested Stacks |
| State Management | CloudFormation | Terraform State | CloudFormation |
| Multi-cloud | ❌ AWS only | ✅ Yes | ❌ AWS only |
| Learning Curve | Low (for .NET devs) | Medium | Medium |
| Bicep Equivalent | ✅ Very similar | Similar | Similar |

### Recommendation: **AWS CDK (C#)**

**Rationale:**
- .NET developers can use familiar C# syntax
- Similar
```

</details>
