---
name: rohioffl__AIREX-AI__database-skill
source: https://github.com/rohioffl/AIREX-AI/blob/0def2b260e34f070bade28b98aca660c0f081c7e/docs/database_skill.md
repo: rohioffl/AIREX-AI
kind: skill
stars: 0
last_pushed: 2026-06-15T12:19:53Z
license: other
score: 9
domains: [backend-api, database, security, devops]
tags: [postgresql, multi-tenancy, rls, audit-log]
curated: 2026-06-15
curated_by: config-scout
---

# rohioffl/AIREX-AI — skill

**Why it's worth keeping:** Enforces strict isolation via composite primary keys + Row Level Security (RLS) and implements a tamper-evident hash chain for audit logs.

**Summary:** Provides a rigorous blueprint for a multi-tenant, auditable PostgreSQL database layer focused on incident management and state machine integrity.

**Source credibility:** High technical depth suggests an expert SRE/Infrastructure origin despite low social proof.

**Recency:** Very current; utilizes modern PostgreSQL 15+ and SQLAlchemy 2.0 patterns.

**Source:** [rohioffl/AIREX-AI/docs/database_skill.md](https://github.com/rohioffl/AIREX-AI/blob/0def2b260e34f070bade28b98aca660c0f081c7e/docs/database_skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: database-core
description: Design and implement the PostgreSQL database layer for the Agentic AI Incident Response Platform. Focus on multi-tenancy, strict schema enforcement, and auditability.
license: Private
---

# Database Skill — AIREX

> **Multi-organization tenancy:** Isolation is still **`tenant_id`-first**. The global **`tenants`** table includes **`organization_id`** (FK to **`organizations`**). Each request uses a tenant-scoped DB session: `SET app.tenant_id` (or equivalent) must reflect the **resolved active tenant** for that request, not a hardcoded UUID. Design migrations and queries for many tenants across many organizations.

This skill defines the data persistence rules for the autonomous SRE system.

This is NOT a schema-less playground.
This is a **System of Record** for production incidents.

The Database must be:

- **Multi-Tenant**: Strict isolation via `tenant_id` and **Row Level Security (RLS)**.
- **Auditable**: Every status change is immutable and hashed.
- **Performant**: Composite Primary Keys for partitioning.
- **Safe**: Database-level Enums and Constraints.

---

## 1. Tech Stack (Mandatory)

| Component | Choice | Restriction |
| :--- | :--
```

</details>
