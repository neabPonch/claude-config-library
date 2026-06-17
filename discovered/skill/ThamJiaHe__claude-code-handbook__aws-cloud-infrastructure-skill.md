---
name: ThamJiaHe__claude-code-handbook__aws-cloud-infrastructure-skill
source: https://github.com/ThamJiaHe/claude-code-handbook/blob/4dedd940c1a2e6bae0a3e98b74bfcb3b8b4a3a3d/skills/examples/aws-cloud-infrastructure-skill.md
repo: ThamJiaHe/claude-code-handbook
kind: skill
stars: 172
last_pushed: 2026-04-19T00:11:57Z
license: mit
score: 8
domains: [cloud-infrastructure, devops, backend-api, security]
tags: [aws, nodejs, deployment, ec2, rds]
curated: 2026-06-15
curated_by: config-scout
---

# ThamJiaHe/claude-code-handbook — skill

**Why it's worth keeping:** The structured multi-step workflow provides a clear execution plan, while specific command templates and anti-patterns prevent common security/operational mistakes.

**Summary:** A comprehensive procedural playbook for deploying Node.js applications on AWS using EC2 and RDS via the AWS CLI.

**Source credibility:** Strong community interest with 172 stars and professional documentation structure.

**Recency:** Current with modern AWS CLI and Node.js standards (despite the future-dated metadata).

**Source:** [ThamJiaHe/claude-code-handbook/skills/examples/aws-cloud-infrastructure-skill.md](https://github.com/ThamJiaHe/claude-code-handbook/blob/4dedd940c1a2e6bae0a3e98b74bfcb3b8b4a3a3d/skills/examples/aws-cloud-infrastructure-skill.md) · 172★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: "AWS Cloud Infrastructure"
description: "Deploy Node.js applications on AWS using EC2, RDS, and managed services with security best practices. Apply when setting up AWS infrastructure, configuring databases, managing security, or optimizing costs."
allowed-tools: Read, Write, Edit, Bash
version: 1.1.0
updated: 2026-01-15
compatibility: Claude Opus 4.5, Claude Code v2.x
---

# AWS Cloud Infrastructure

Systematic AWS deployment for Node.js applications ensuring scalability, security, and cost efficiency.

## Overview

This Skill enforces:
- EC2 instance configuration and security
- RDS (Relational Database Service) setup
- IAM roles and least-privilege access
- Environment variable and secrets management
- Auto-scaling and load balancing
- Security group and network configuration
- CloudWatch monitoring

Apply when deploying to AWS, configuring databases, or managing cloud infrastructure.

## Deployment Workflow

**Every AWS deployment follows this process**:

```
Step 1: Create EC2 Instance
  ↓
Step 2: Configure Security Groups
  ↓
Step 3: Install Node.js and dependencies
  ↓
Step 4: Deploy application with PM2
  ↓
Step 5: Set up RDS database
  ↓
Step 6: Configure environ
```

</details>
