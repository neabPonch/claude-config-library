---
name: cartography-cncf__cartography__skill
source: https://github.com/cartography-cncf/cartography/blob/c0dca9a3c2cdeab6adc3268b7f0d071fc6ace7bc/.agents/skills/create-rule/SKILL.md
repo: cartography-cncf/cartography
kind: skill
stars: 3923
last_pushed: 2026-06-13T18:04:09Z
license: apache-2.0
score: 9
domains: [security, infrastructure-as-code, data-engineering, cli-tools]
tags: [template, rule-authoring, security-automation]
curated: 2026-06-15
curated_by: config-scout
---

# cartography-cncf/cartography — skill

**Why it's worth keeping:** It details critical constraints like field aliasing requirements and the specific order required for finding title derivation. The step-by-step template approach makes it highly actionable for an agent.

**Summary:** A rigorous technical specification for authoring security rules in Cartography via Cypher facts and Pydantic models.

**Source credibility:** The source (Cartography) is a high-star, actively maintained CNCF project used for infrastructure security.

**Recency:** Current; utilizes modern Python type hinting and Pydantic patterns common in today's development environments.

**Source:** [cartography-cncf/cartography/.agents/skills/create-rule/SKILL.md](https://github.com/cartography-cncf/cartography/blob/c0dca9a3c2cdeab6adc3268b7f0d071fc6ace7bc/.agents/skills/create-rule/SKILL.md) · 3923★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: create-rule
description: Author a Cartography security rule (one or more Cypher Facts plus a Pydantic Finding output model) under `cartography/rules/data/rules/`. Use when the user asks to add a security check, detection, attack-surface query, compliance control, CIS benchmark rule, or cross-cloud detection.
---

# create-rule

Cartography rules detect attack surfaces, security gaps, and compliance issues across the graph. Rules are composed of one or more Facts (Cypher queries) and a Finding output model (Pydantic).

## Architecture

```
Rule (e.g., "database-exposed")
  ├─ Fact (e.g., "aws-rds-public")
  ├─ Fact (e.g., "azure-sql-public")
  └─ Fact (e.g., "gcp-cloudsql-public")
```

- **Rule** — represents a security issue / attack surface.
- **Fact** — single Cypher query that gathers evidence.
- **Finding** — Pydantic model defining the result row structure.

## Critical rules

1. **`cypher_query` aliases must match `Finding` field names exactly.** Use `RETURN x.id AS id, x.name AS name`.
2. **`cypher_visual_query` returns nodes**, not properties — used for graph viz.
3. **All `Finding` fields are `| None` with default `None`.** The `source` field is auto-populated.
4
```

</details>
