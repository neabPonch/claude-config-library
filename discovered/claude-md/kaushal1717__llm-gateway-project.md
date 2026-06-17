---
name: kaushal1717__llm-gateway-project
source: https://github.com/kaushal1717/llm-gateway-project/blob/51433127127b727a9608c92669bfcf6a6e79cee7/claude.md
repo: kaushal1717/llm-gateway-project
kind: claude-md
stars: 0
last_pushed: 2026-02-03T05:32:57Z
license: unknown
score: 9
domains: [cloud-infrastructure, backend-api, devsecops, ai-infrastructure]
tags: [aws, terraform, llm-gateway, security]
curated: 2026-06-16
curated_by: config-scout
---

# kaushal1717/llm-gateway-project — claude-md

**Why it's worth keeping:** The 'Critical Operational Constraints' section is a masterclass in providing 'failure-preventing' instructions (e.g., the DB connection pool limit) which prevents the AI from making costly architectural errors.

**Summary:** A highly structured project context file for an AWS-based LLM gateway that provides specific mapping logic and hardware constraints.

**Source credibility:** Low visibility repo, likely a single developer/MVP project.

**Recency:** Very current; includes modern model identifiers and recent AWS patterns.

**Source:** [kaushal1717/llm-gateway-project/claude.md](https://github.com/kaushal1717/llm-gateway-project/blob/51433127127b727a9608c92669bfcf6a6e79cee7/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project Context: Enterprise LLM Gateway (MVP)

## 1. Mission Statement

Build a cost-efficient, secure Generative AI Gateway on AWS to centralize API access for 100 users. The system must enforce strict monthly budgets and role-based model access using AWS Bedrock as the sole provider.

## 2. Technical Stack

- **Proxy Software:** LiteLLM (Python/Docker).
- **Cloud Provider:** AWS (Region: ap-south-1).
- **IaC:** Terraform (Modular architecture).
- **Compute:** AWS ECS Fargate (Spot Capacity preferred for cost).
- **Database:** AWS RDS PostgreSQL (db.t4g.micro).
- **Secrets:** AWS Secrets Manager.

## 3. User Governance Tiers

The application must enforce these exact tiers via Virtual Keys:

| **Tier Name** | **Budget (Monthly)** | **Rate Limit** | **Allowed Models (Logical)** |
| :-----------: | :------------------: | :------------: | :--------------------------: |
| **Drafting**  |        $2.00         |     10 RPM     |         model-cheap          |
|  **Coding**   |        $20.00        |     50 RPM     |        model-balanced        |
| **Architect** |       $500.00        |    100 RPM     |       model-reasoning        |

## 4. Model Mapping (AWS Bedrock)

Map the logical
```

</details>
