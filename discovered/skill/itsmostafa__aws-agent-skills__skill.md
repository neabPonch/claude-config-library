---
name: itsmostafa__aws-agent-skills__skill
source: https://github.com/itsmostafa/aws-agent-skills/blob/4ab904a69cda893b5c98f97966bf9a48311823e9/skills/rds/SKILL.md
repo: itsmostafa/aws-agent-skills
kind: skill
stars: 1127
last_pushed: 2026-06-15T11:02:29Z
license: mit
score: 9
domains: [cloud-infrastructure, devops, aws, database]
tags: [rds, aws-cli, boto3, provisioning]
curated: 2026-06-15
curated_by: config-scout
---

# itsmostafa/aws-agent-skills — skill

**Why it's worth keeping:** It provides multi-step orchestration patterns (Subnet -> Security Group -> Instance) rather than isolated commands, which is essential for successful agentic execution. The inclusion of both CLI and Python/Boto3 examples makes it versatile for different automation environments.

**Summary:** A highly actionable technical manual for managing AWS RDS via CLI and Boto3. It covers end-to-end provisioning workflows including networking dependencies.

**Source credibility:** High; the repository has significant community traction with 1k+ stars and very recent updates.

**Recency:** Very current, referencing modern AWS features like gp3 storage and PostgreSQL 16.x.

**Source:** [itsmostafa/aws-agent-skills/skills/rds/SKILL.md](https://github.com/itsmostafa/aws-agent-skills/blob/4ab904a69cda893b5c98f97966bf9a48311823e9/skills/rds/SKILL.md) · 1127★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: rds
description: AWS RDS relational database service for managed databases. Use when provisioning databases, configuring backups, managing replicas, troubleshooting connectivity, or optimizing performance.
last_updated: "2026-01-07"
doc_source: https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/
---

# AWS RDS

Amazon Relational Database Service (RDS) provides managed relational databases including MySQL, PostgreSQL, MariaDB, Oracle, SQL Server, and Aurora. RDS handles provisioning, patching, backups, and failover.

## Table of Contents

- [Core Concepts](#core-concepts)
- [Common Patterns](#common-patterns)
- [CLI Reference](#cli-reference)
- [Best Practices](#best-practices)
- [Troubleshooting](#troubleshooting)
- [References](#references)

## Core Concepts

### DB Instance Classes

| Category | Example | Use Case |
|----------|---------|----------|
| Standard | db.m6g.large | General purpose |
| Memory Optimized | db.r6g.large | High memory workloads |
| Burstable | db.t3.medium | Variable workloads, dev/test |

### Storage Types

| Type | IOPS | Use Case |
|------|------|----------|
| gp3 | 3,000-16,000 | Most workloads |
| io1/io2 | Up to 256,000 | High-performan
```

</details>
