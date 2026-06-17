---
name: alirezarezvani__claude-skills__skill
source: https://github.com/alirezarezvani/claude-skills/blob/4a3c05b69e64f4925f7fc65c88890f614f79caf0/engineering-team/skills/aws-solution-architect/SKILL.md
repo: alirezarezvani/claude-skills
kind: skill
stars: 18200
last_pushed: 2026-06-12T05:59:36Z
license: mit
score: 9
domains: [cloud-infrastructure, devops, aws]
tags: [aws, iac, serverless, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# alirezarezvani/claude-skills — skill

**Why it's worth keeping:** It defines highly structured tool interactions via JSON examples and includes a crucial 'Validation/Failure' phase that makes the agent more reliable during real deployments.

**Summary:** A rigorous, multi-step workflow for designing and deploying AWS architectures using IaC. It covers the entire lifecycle from requirement gathering to cost optimization and failure recovery.

**Source credibility:** High; the source repository is heavily starred (18k+) and shows active maintenance.

**Recency:** Current; utilizes modern runtimes like Nodejs 20.x and contemporary AWS serverless patterns.

**Source:** [alirezarezvani/claude-skills/engineering-team/skills/aws-solution-architect/SKILL.md](https://github.com/alirezarezvani/claude-skills/blob/4a3c05b69e64f4925f7fc65c88890f614f79caf0/engineering-team/skills/aws-solution-architect/SKILL.md) · 18200★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: "aws-solution-architect"
description: Design AWS architectures for startups using serverless patterns and IaC templates. Use when asked to design serverless architecture, create CloudFormation templates, optimize AWS costs, set up CI/CD pipelines, or migrate to AWS. Covers Lambda, API Gateway, DynamoDB, ECS, Aurora, and cost optimization.
---

# AWS Solution Architect

Design scalable, cost-effective AWS architectures for startups with infrastructure-as-code templates.

---

## Workflow

### Step 1: Gather Requirements

Collect application specifications:

```
- Application type (web app, mobile backend, data pipeline, SaaS)
- Expected users and requests per second
- Budget constraints (monthly spend limit)
- Team size and AWS experience level
- Compliance requirements (GDPR, HIPAA, SOC 2)
- Availability requirements (SLA, RPO/RTO)
```

### Step 2: Design Architecture

Run the architecture designer to get pattern recommendations:

```bash
python scripts/architecture_designer.py --input requirements.json
```

**Example output:**

```json
{
  "recommended_pattern": "serverless_web",
  "service_stack": ["S3", "CloudFront", "API Gateway", "Lambda", "DynamoDB", "Cognito"],
  "
```

</details>
