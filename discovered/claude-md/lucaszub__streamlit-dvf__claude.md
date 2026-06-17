---
name: lucaszub__streamlit-dvf__claude
source: https://github.com/lucaszub/streamlit-dvf/blob/d8e48ca22cd7821812d367229b25cf3256075860/.claude.md
repo: lucaszub/streamlit-dvf
kind: claude-md
stars: 0
last_pushed: 2026-01-17T08:39:53Z
license: unknown
score: 9
domains: [data-engineering, sql]
tags: [semantic-layer, schema-definition, snowflake]
curated: 2026-06-15
curated_by: config-scout
---

# lucaszub/streamlit-dvf — claude-md

**Why it's worth keeping:** It provides 'Common Query Patterns' which give the AI logic templates to follow, and uses sample values to clarify categorical data formats.

**Summary:** A comprehensive semantic layer definition for a Snowflake data warehouse featuring dimensions, facts, and relationship mappings.

**Source credibility:** Low GitHub stars, but the highly specific technical detail suggests it is a real-world schema documentation rather than a template.

**Recency:** Highly current; this level of detail is exactly what modern LLMs need for accurate SQL generation.

**Source:** [lucaszub/streamlit-dvf/.claude.md](https://github.com/lucaszub/streamlit-dvf/blob/d8e48ca22cd7821812d367229b25cf3256075860/.claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# DVF (Demandes de Valeurs Foncières) - Snowflake Semantic Layer

This project analyzes French real estate transaction data using a Snowflake data warehouse.

## Database Structure

**Database**: VALFONC_ANALYTICS
**Schema**: GOLD

## Data Model Overview

The semantic model follows a star schema with dimension tables and a central fact table for real estate mutations (transactions).

---

## Dimension Tables

### DIM_ADDRESS
**Primary Key**: ADDRESS_ID

Physical street addresses including street numbers, street names, postal codes, and city names in France.

**Key Fields**:
- `ADDRESS_ID`: Unique identifier for each address record
- `ADDRESS`: Full physical street address
- `NO_VOIE`: Street number or building number
- `TYPE_DE_VOIE`: Type of street (ACH, AV, CHS, etc.)
- `VOIE`: Street name
- `CODE_POSTAL`: Postal code
- `COMMUNE`: French commune name (smallest administrative division)
- `CODE_DEPARTEMENT`: French department code (administrative division)
- `CREATED_AT`: Timestamp when the record was created

**Sample Values**:
- TYPE_DE_VOIE: "ACH", "AV", "CHS"
- CODE_DEPARTEMENT: "36", "78", "44"
- COMMUNE: "MONT-DE-MARSAN", "SUCCIEU", "ALFORTVILLE"

---

### DIM_CODE_POSTAL
**P
```

</details>
