---
name: phuryn__pm-skills__skill
source: https://github.com/phuryn/pm-skills/blob/d384f0c9eb81fe74656a4f6da168587836939edb/pm-data-analytics/skills/sql-queries/SKILL.md
repo: phuryn/pm-skills
kind: skill
stars: 18326
last_pushed: 2026-06-06T14:12:26Z
license: mit
score: 7
domains: [data-analysis, database]
tags: [sql, query-generation, data-engineering]
curated: 2026-06-15
curated_by: config-scout
---

# phuryn/pm-skills — skill

**Why it's worth keeping:** The 'How It Works' section establishes a reliable reasoning chain (Analyze -> Clarify -> Generate) that prevents hallucinations by forcing context gathering before code writing.

**Summary:** Defines a rigorous multi-step protocol for translating natural language into dialect-specific SQL through schema analysis and clarification.

**Source credibility:** Highly credible; the source repository is widely recognized with high engagement/stars.

**Recency:** Current; follows modern agentic workflow patterns for LLMs.

**Source:** [phuryn/pm-skills/pm-data-analytics/skills/sql-queries/SKILL.md](https://github.com/phuryn/pm-skills/blob/d384f0c9eb81fe74656a4f6da168587836939edb/pm-data-analytics/skills/sql-queries/SKILL.md) · 18326★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: sql-queries
description: "Generate SQL queries from natural language descriptions. Supports BigQuery, PostgreSQL, MySQL, and other dialects. Reads database schemas from uploaded diagrams or documentation. Use when writing SQL, building data reports, exploring databases, or translating business questions into queries."
---

# SQL Query Generator

## Purpose
Transform natural language requirements into optimized SQL queries across multiple database platforms. This skill helps product managers, analysts, and engineers generate accurate queries without manual syntax work.

## How It Works

### Step 1: Understand Your Database Schema
- If you provide a schema file (SQL, documentation, or diagram description), I will read and analyze it
- Extract table names, column definitions, data types, and relationships
- Identify primary keys, foreign keys, and indexing strategies

### Step 2: Process Your Request
- Clarify the exact data you need to retrieve or analyze
- Confirm the SQL dialect (BigQuery, PostgreSQL, MySQL, Snowflake, etc.)
- Ask for any additional requirements (filters, aggregations, sorting)

### Step 3: Generate Optimized Query
- Write efficient SQL that leverages you
```

</details>
