---
name: onesphereai__hotdoc-alternate
source: https://github.com/onesphereai/hotdoc-alternate/blob/78f7537d7b748b68ee8ed8f622fb2485b31095b2/Claude.md
repo: onesphereai/hotdoc-alternate
kind: claude-md
stars: 0
last_pushed: 2025-08-12T10:06:12Z
license: unknown
score: 9
domains: [backend-api, aws-serverless, infrastructure-as-code]
tags: [aws, serverless, healthcare, roadmap, multitenancy]
curated: 2026-06-14
curated_by: config-scout
---

# onesphereai/hotdoc-alternate — claude-md

**Why it's worth keeping:** Features explicit DynamoDB partition/sort key schemas, multi-tenancy isolation rules, and strict compliance guardrails that prevent agent drift in architectural decisions.

**Summary:** A highly detailed blueprint for building a cloud-native healthcare MVP using AWS Serverless and React.

**Source credibility:** Low star count but demonstrates high technical density and professional structural planning.

**Recency:** 10 months old; still highly relevant for modern AWS serverless patterns.

**Source:** [onesphereai/hotdoc-alternate/Claude.md](https://github.com/onesphereai/hotdoc-alternate/blob/78f7537d7b748b68ee8ed8f622fb2485b31095b2/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
claude.md — HotDoc‑Alternate MVP Plan (React + AWS Serverless)

**Purpose:** This document instructs Claude Code to build an MVP in phased increments for a HotDoc‑like product. It includes scope, milestones, repo layout, Infrastructure as Code (IaC), API contracts, data models, test plans, and agent-ready tasks/prompts. The stack is **React (Vite) + AWS Serverless** (API Gateway, Lambda, Cognito, DynamoDB, EventBridge, SQS, SNS/Pinpoint, Step Functions, Amazon Connect) with **AWS SAM** for IaC. All technical choices and deliverables are explicit and actionable for each MVP phase.

⸻

0) Non‑functional Guardrails (Read First)
	•	**Compliance (AU context):** Adhere to Australian Privacy Act 1988 (APPs). No clinical notes or pathology in MVP; store only booking metadata and basic demographics. All PII is encrypted at rest using AWS KMS and in transit using TLS 1.2+.
	•	**Security:** Use AWS Cognito User Pools for patients and practice admins. Use Cognito Identity Pools (optional) for pre‑signed S3 uploads. Enforce principle of least privilege via IAM roles and policies. Store all secrets in AWS SSM Parameter Store.
	•	**Observability:** Use AWS CloudWatch for logs and metrics, AWS X-R
```

</details>
