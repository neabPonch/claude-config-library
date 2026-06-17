---
name: Snowflake-Labs__cocoplus__personas-skill
source: https://github.com/Snowflake-Labs/cocoplus/blob/81eb1b97405686c99a896f78cc9c291e6d33a3c9/.cortex/skills/personas.skill.md
repo: Snowflake-Labs/cocoplus
kind: skill
stars: 604
last_pushed: 2026-06-14T17:06:29Z
license: mit
score: 8
domains: [data-engineering, cli-tools, agents-ai]
tags: [persona-catalog, meta-skill]
curated: 2026-06-16
curated_by: config-scout
---

# Snowflake-Labs/cocoplus — skill

**Why it's worth keeping:** Uses 'Anti-Rationalization' to prevent output truncation and 'Exit Criteria' for quality control—crucial patterns for high-fidelity reference skills.

**Summary:** Acts as a specialized discovery tool to display the full catalog of personas, triggers, and tools available within the CocoPlus ecosystem.

**Source credibility:** High; developed by Snowflake Labs with highly active maintenance.

**Recency:** Current; updated within the last month.

**Source:** [Snowflake-Labs/cocoplus/.cortex/skills/personas.skill.md](https://github.com/Snowflake-Labs/cocoplus/blob/81eb1b97405686c99a896f78cc9c291e6d33a3c9/.cortex/skills/personas.skill.md) · 604★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: "personas"
description: "List all available CocoPlus specialist personas with their triggers, models, modes, and locked tool sets. No preconditions required — works without $pod init."
version: "1.0.0"
author: "CocoPlus"
tags:
  - cocoplus
  - personas
---

Your objective is to display the complete CocoPlus persona catalog.

Output the following table:

```
# Available Personas

| Persona | Trigger | Model | Mode | Isolation | Tools |
|---------|---------|-------|------|-----------|-------|
| Data Engineer | $de | sonnet | auto | worktree | SnowflakeSqlExecute, DataDiff, Bash, Read, Write, Edit |
| Analytics Engineer | $ae | sonnet | auto | none | SnowflakeSqlExecute, ReflectSemanticModel, Read, Write, Edit |
| Data Scientist | $ds | sonnet | auto | none | NotebookExecute, SnowflakeSqlExecute, Bash, Read, Write |
| Data Analyst | $da | haiku | auto | none | SnowflakeSqlExecute, SnowflakeMultiCortexAnalyst, Read |
| BI Analyst | $bi | haiku | auto | none | ReflectSemanticModel, SnowflakeMultiCortexAnalyst, Read |
| Data Product Manager | $dpm | sonnet | plan | none | Read, Write, SnowflakeProductDocs |
| Data Steward | $dst | sonnet | plan | none | SnowflakeSqlExecute, Dat
```

</details>
