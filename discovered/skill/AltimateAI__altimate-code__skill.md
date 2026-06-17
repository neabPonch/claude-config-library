---
name: AltimateAI__altimate-code__skill
source: https://github.com/AltimateAI/altimate-code/blob/3a8d1c0f6c99d95453ee92cc74c5182d45cf69fe/.opencode/skills/pii-audit/SKILL.md
repo: AltimateAI/altimate-code
kind: skill
stars: 674
last_pushed: 2026-06-15T04:02:32Z
license: mit
score: 9
domains: [data-engineering, security, compliance, sql]
tags: [pii, audit, dbt, compliance]
curated: 2026-06-15
curated_by: config-scout
---

# AltimateAI/altimate-code — skill

**Why it's worth keeping:** It includes critical 'Do NOT use' constraints to prevent misuse and provides a highly specific report template that ensures consistent, professional output structure.

**Summary:** This skill automates the detection of PII in database schemas and audits dbt models for compliance risk. It provides structured workflows for both static schema analysis and live warehouse inspection.

**Source credibility:** High; AltimateAI is a well-maintained source with significant GitHub traction for data engineering tools.

**Recency:** Very current; follows modern agentic prompting techniques like branched options (Option A vs Option B).

**Source:** [AltimateAI/altimate-code/.opencode/skills/pii-audit/SKILL.md](https://github.com/AltimateAI/altimate-code/blob/3a8d1c0f6c99d95453ee92cc74c5182d45cf69fe/.opencode/skills/pii-audit/SKILL.md) · 674★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pii-audit
description: Classify schema columns for PII (SSN, email, phone, name, address, credit card) and check whether queries expose them. Use for GDPR/CCPA/HIPAA compliance audits.
---

# PII Audit

## Requirements
**Agent:** any (read-only analysis)
**Tools used:** altimate_core_classify_pii, altimate_core_query_pii, schema_detect_pii, schema_inspect, read, glob

## When to Use This Skill

**Use when the user wants to:**
- Scan a database schema for PII columns (SSN, email, phone, name, address, credit card, IP)
- Check if a specific query exposes PII data
- Audit dbt models for PII leakage before production deployment
- Generate a PII inventory for compliance (GDPR, CCPA, HIPAA)

**Do NOT use for:**
- SQL injection scanning -> use `sql-review`
- General SQL quality checks -> use `sql-review`
- Access control auditing -> finops role tools in `cost-report`

## Workflow

### 1. Classify Schema for PII

**Option A — From schema YAML/JSON:**

```
altimate_core_classify_pii(schema_context: <schema_object>)
```

Analyzes column names, types, and patterns to detect PII categories:
- **Direct identifiers**: SSN, email, phone, full name, credit card number
- **Quasi-identifie
```

</details>
