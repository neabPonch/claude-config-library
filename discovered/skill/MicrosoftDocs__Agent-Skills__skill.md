---
name: MicrosoftDocs__Agent-Skills__skill
source: https://github.com/MicrosoftDocs/Agent-Skills/blob/49f3b3eb2545a278491122c6bbed516e532cb1b4/skills/azure-cosmos-db/SKILL.md
repo: MicrosoftDocs/Agent-Skills
kind: skill
stars: 610
last_pushed: 2026-06-14T02:40:30Z
license: cc-by-4.0
score: 9
domains: [cloud-infrastructure, database]
tags: [structured-knowledge, documentation-mapping, azure]
curated: 2026-06-15
curated_by: config-scout
---

# MicrosoftDocs/Agent-Skills — skill

**Why it's worth keeping:** The 'Category Index' pattern using line-range pointers (e.g., L37-L90) allows an agent to surgically retrieve only relevant sections, maximizing context window efficiency for large docs.

**Summary:** A highly structured skill file that maps documentation categories to specific line ranges and external resource links.

**Source credibility:** Highly credible; official Microsoft documentation repository.

**Recency:** Current; includes modern tool fallback patterns and MCP integration instructions.

**Source:** [MicrosoftDocs/Agent-Skills/skills/azure-cosmos-db/SKILL.md](https://github.com/MicrosoftDocs/Agent-Skills/blob/49f3b3eb2545a278491122c6bbed516e532cb1b4/skills/azure-cosmos-db/SKILL.md) · 610★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: azure-cosmos-db
description: Expert knowledge for Azure Cosmos DB development including troubleshooting, best practices, decision making, architecture & design patterns, limits & quotas, security, configuration, integrations & coding patterns, and deployment. Use when building Cosmos DB NoSQL/Mongo/Cassandra apps, using change feed, multi-region, vector search, or AI/RAG, and other Azure Cosmos DB related development tasks. Not for Azure Table Storage (use azure-table-storage), Azure SQL Database (use azure-sql-database), Azure SQL Managed Instance (use azure-sql-managed-instance), Azure Data Explorer (use azure-data-explorer).
compatibility: Requires network access. Uses mcp_microsoftdocs:microsoft_docs_fetch or fetch_webpage to retrieve documentation.
metadata:
  generated_at: "2026-06-07"
  generator: "docs2skills/1.0.0"
---
# Azure Cosmos DB Skill

This skill provides expert guidance for Azure Cosmos DB. Covers troubleshooting, best practices, decision making, architecture & design patterns, limits & quotas, security, configuration, integrations & coding patterns, and deployment. It combines local quick-reference content with remote documentation fetching capabilities
```

</details>
