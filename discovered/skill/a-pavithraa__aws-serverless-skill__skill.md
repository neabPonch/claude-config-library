---
name: a-pavithraa__aws-serverless-skill__skill
source: https://github.com/a-pavithraa/aws-serverless-skill/blob/2b66211e7baa318c10d072be127c3f071c4ebee2/skills/aws-dynamodb/SKILL.md
repo: a-pavithraa/aws-serverless-skill
kind: skill
stars: 8
last_pushed: 2026-02-25T11:40:24Z
license: unknown
score: 9
domains: [backend-api, cloud-infrastructure, database-design]
tags: [aws, dynamodb, serverless, terraform, data-modeling]
curated: 2026-06-16
curated_by: config-scout
---

# a-pavithraa/aws-serverless-skill — skill

**Why it's worth keeping:** The 'Critical Anti-Patterns' section offers high-value technical guardrails, while the decision tables provide clear logic branches for agentic reasoning. The specific advice on zero-padding sort keys and GSI optimization is highly transferable.

**Summary:** Provides expert-level AWS DynamoDB architectural patterns, anti-patterns, and decision frameworks for data modeling and schema migrations.

**Source credibility:** Moderate; 8 stars indicates a niche but respected utility in the serverless community.

**Recency:** Highly current; includes very recent Terraform provider updates and forward-looking AWS feature notes.

**Source:** [a-pavithraa/aws-serverless-skill/skills/aws-dynamodb/SKILL.md](https://github.com/a-pavithraa/aws-serverless-skill/blob/2b66211e7baa318c10d072be127c3f071c4ebee2/skills/aws-dynamodb/SKILL.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: aws-dynamodb
description: "Patterns and best practices for Amazon DynamoDB data modeling and access patterns. Use when the user asks about DynamoDB table design, single-table design, GSIs, multi-attribute composite keys, one-to-many relationships, cost optimization, or Terraform DynamoDB resources. Triggers on: DynamoDB, single-table design, GSI, partition key, sort key, access patterns, filter expressions, TTL, vertical sharding, composite keys, multi-attribute keys."
---

# AWS DynamoDB

## Quick Reference

> All patterns are in [`references/dynamodb-patterns.md`](references/dynamodb-patterns.md).

| Topic | Key Insight |
|-------|-------------|
| Data modeling | Design access patterns FIRST, schema second |
| Single-table design | Items queried together live together |
| GSIs | Multi-attribute composite keys avoid synthetic key hacks |
| Cost optimization | Filter expressions do NOT reduce read costs |
| Sort order control | `#` prefix positions parent at sort boundary; numeric difference enables reverse integer ordering |
| Sparse indexes | Entity-type filter (always-on attr) vs conditional filter (add/remove attr on state change) |
| Reference counts | TransactWriteI
```

</details>
