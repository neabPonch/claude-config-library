---
name: agentic-community__mcp-gateway-registry__skill
source: https://github.com/agentic-community/mcp-gateway-registry/blob/3d44f0382d0a9c676f65878e5f012193c21c08a0/.claude/skills/terraform-setup/SKILL.md
repo: agentic-community/mcp-gateway-registry
kind: skill
stars: 705
last_pushed: 2026-06-14T22:33:50Z
license: apache-2.0
score: 9
domains: [infrastructure-as-code, devops, cloud-deployment, aws]
tags: [terraform, aws, orchestration, deployment]
curated: 2026-06-15
curated_by: config-scout
---

# agentic-community/mcp-gateway-registry — skill

**Why it's worth keeping:** Uses a 'Step 0' mandatory interaction pattern to prevent accidental/expensive execution, implements a formal step-tracking log for observability, and provides proactive financial risk disclosures.

**Summary:** A highly sophisticated skill designed to orchestrate a complex AWS infrastructure deployment via Terraform. It handles environment detection, toolchain bootstrapping, and cost-risk transparency.

**Source credibility:** High; part of an active, highly-starred enterprise MCP project.

**Recency:** Current; uses modern toolchain patterns like 'uv'.

**Source:** [agentic-community/mcp-gateway-registry/.claude/skills/terraform-setup/SKILL.md](https://github.com/agentic-community/mcp-gateway-registry/blob/3d44f0382d0a9c676f65878e5f012193c21c08a0/.claude/skills/terraform-setup/SKILL.md) · 705★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: terraform-setup
description: "Install (deploy) MCP Gateway & Registry on AWS using the Terraform aws-ecs stack (ECS Fargate, Aurora, DocumentDB, Keycloak). Asks whether you are running from an EC2 instance or a local laptop, confirms the required AWS IAM permissions are in place, clones the repository, bootstraps the toolchain (uv, AWS CLI, Terraform), configures terraform.tfvars, runs the two-stage terraform apply, and completes post-deployment setup. Does NOT create IAM roles itself — it tells you the permissions you need and offers to guide you through setting them up."
license: Apache-2.0
metadata:
  author: mcp-gateway-registry
  version: "1.0"
---

# MCP Gateway & Registry — Terraform (AWS ECS) Install Skill

**Repository:** https://github.com/agentic-community/mcp-gateway-registry
**This skill:** https://github.com/agentic-community/mcp-gateway-registry/blob/main/.claude/skills/terraform-setup/SKILL.md
**Full Terraform guide:** https://github.com/agentic-community/mcp-gateway-registry/blob/main/terraform/aws-ecs/README.md

## How to run this skill without cloning the repository

This skill is self-contained. You can invoke it from any directory in Claude Code. It w
```

</details>
