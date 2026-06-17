---
name: j4flmao__agent-skills__skill
source: https://github.com/j4flmao/agent-skills/blob/c202578db02bfa1e3abf2c4a9e6a7c6dc129a433/skills/devops/aws/SKILL.md
repo: j4flmao/agent-skills
kind: skill
stars: 8
last_pushed: 2026-06-05T09:02:36Z
license: mit
score: 9
domains: [devops, cloud-infrastructure, iac]
tags: [aws, terraform, architecture]
curated: 2026-06-17
curated_by: config-scout
---

# j4flmao/agent-skills — skill

**Why it's worth keeping:** The 'Architecture Decision Trees' provide explicit logic for service selection (e.g., Compute/Database) which significantly reduces LLM hallucinations, while the strict response format is perfect for agentic tool-use.

**Summary:** A high-density DevOps skill file providing structured architectural decision trees and strict output protocols for AWS infrastructure automation.

**Source credibility:** Moderate; a niche repository with active maintenance.

**Recency:** Highly current; utilizes modern IaC patterns and advanced prompting structures relevant to Claude Code.

**Source:** [j4flmao/agent-skills/skills/devops/aws/SKILL.md](https://github.com/j4flmao/agent-skills/blob/c202578db02bfa1e3abf2c4a9e6a7c6dc129a433/skills/devops/aws/SKILL.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: aws
description: >
  Use this skill when the user says 'AWS', 'EC2', 'S3', 'RDS', 'Lambda', 'VPC',
  'IAM', 'Well-Architected', 'cost optimization', 'CloudFormation',
  'Terraform AWS', 'EKS', 'ECS', 'ELB', 'Route53', 'CloudFront', 'WAF',
  'Auto Scaling', 'Security Group', 'NACL', 'AWS CLI', 'AWS SDK',
  'boto3', 'aws-vault', 'SSM', 'Secrets Manager', 'KMS', 'CloudWatch'.
  Covers: compute selection (EC2 vs Lambda vs ECS vs EKS), IAM policies,
  networking patterns, Well-Architected Framework, cost optimization,
  security best practices, multi-account strategy.
  Do NOT use for: GCP, Azure, Alibaba Cloud.
version: "2.0.0"
author: "j4flmao"
license: "MIT"
compatibility:
  claude-code: true
  cursor: true
  codex: true
  windsurf: true
tags: [devops, aws, cloud, infrastructure, phase-5]
---

# AWS

## Purpose
Design, deploy, and manage AWS infrastructure following the Well-Architected Framework with service decision trees, networking patterns, security best practices, and cost optimization.

## Agent Protocol

### Trigger
Exact user phrases: "AWS", "EC2", "S3", "RDS", "Lambda", "VPC", "IAM", "Well-Architected", "cost optimization", "CloudFormation", "Terraform AWS", "EKS"
```

</details>
