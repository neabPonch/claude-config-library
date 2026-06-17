---
name: MoizIbnYousaf__Ai-Agent-Skills__skill
source: https://github.com/MoizIbnYousaf/Ai-Agent-Skills/blob/039ad59e2a1256a47c08abc7d2c194446e9a2c02/skills/database-design/SKILL.md
repo: MoizIbnYousaf/Ai-Agent-Skills
kind: skill
stars: 1073
last_pushed: 2026-05-05T09:57:12Z
license: mit
score: 8
domains: [database, backend]
tags: [postgres, sql, migrations, optimization]
curated: 2026-06-15
curated_by: config-scout
---

# MoizIbnYousaf/Ai-Agent-Skills — skill

**Why it's worth keeping:** Provides specific PostgreSQL observability queries and a repeatable multi-step workflow for zero-downtime migrations.

**Summary:** A high-quality technical reference for schema design, index optimization, and safe database migrations.

**Source credibility:** High-star curated repository indicating reliable content curation.

**Recency:** Aligns with modern high-availability database management standards.

**Source:** [MoizIbnYousaf/Ai-Agent-Skills/skills/database-design/SKILL.md](https://github.com/MoizIbnYousaf/Ai-Agent-Skills/blob/039ad59e2a1256a47c08abc7d2c194446e9a2c02/skills/database-design/SKILL.md) · 1073★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: database-design
description: Database schema design, optimization, and migration patterns for PostgreSQL, MySQL, and NoSQL databases. Use for designing schemas, writing migrations, or optimizing queries.
source: wshobson/agents
license: MIT
version: 4.1.0
---

# Database Design

## Schema Design Principles

### Normalization Guidelines
```sql
-- 1NF: Atomic values, no repeating groups
-- 2NF: No partial dependencies on composite keys
-- 3NF: No transitive dependencies

-- Users table (normalized)
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  email VARCHAR(255) UNIQUE NOT NULL,
  created_at TIMESTAMPTZ DEFAULT NOW()
);

-- Addresses table (separate entity)
CREATE TABLE addresses (
  id SERIAL PRIMARY KEY,
  user_id INTEGER REFERENCES users(id) ON DELETE CASCADE,
  street VARCHAR(255),
  city VARCHAR(100),
  country VARCHAR(100),
  is_primary BOOLEAN DEFAULT false
);
```

### Denormalization for Performance
```sql
-- When read performance matters more than write consistency
CREATE TABLE order_summaries (
  id SERIAL PRIMARY KEY,
  order_id INTEGER REFERENCES orders(id),
  customer_name VARCHAR(255),  -- Denormalized from customers
  total_amount DECIMAL(10,2),
  item_coun
```

</details>
