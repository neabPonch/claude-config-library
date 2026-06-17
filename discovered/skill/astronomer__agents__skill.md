---
name: astronomer__agents__skill
source: https://github.com/astronomer/agents/blob/da0048c49f88335c9d9cc617837e182ba04a2ab5/skills/cosmos-dbt-core/SKILL.md
repo: astronomer/agents
kind: skill
stars: 391
last_pushed: 2026-06-15T18:32:22Z
license: apache-2.0
score: 9
domains: [data-engineering, orchestration, airflow]
tags: [dbt, cosmos, dag, taskgroup]
curated: 2026-06-16
curated_by: config-scout
---

# astronomer/agents — skill

**Why it's worth keeping:** Uses highly effective comparison tables that convert complex configuration choices (parsing/execution modes) into actionable 'if-then' logic. The modular structure mirrors the actual object hierarchy of the library, making it a perfect template for agentic tool use.

**Summary:** A decision-tree driven guide for configuring Astronomer Cosmos to integrate dbt Core into Airflow DAGs or TaskGroups.

**Source credibility:** High; authored by Astronomer, the leading authority on Airflow and Cosmos.

**Recency:** Very current; includes support for Airflow 3.x and latest Cosmos versions.

**Source:** [astronomer/agents/skills/cosmos-dbt-core/SKILL.md](https://github.com/astronomer/agents/blob/da0048c49f88335c9d9cc617837e182ba04a2ab5/skills/cosmos-dbt-core/SKILL.md) · 391★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cosmos-dbt-core
description: Use when turning a dbt Core project into an Airflow DAG/TaskGroup using Astronomer Cosmos. Does not cover dbt Fusion. Before implementing, verify dbt engine, warehouse, Airflow version, execution environment, DAG vs TaskGroup, and manifest availability.
---

# Cosmos + dbt Core: Implementation Checklist

Execute steps in order. Prefer the simplest configuration that meets the user's constraints.

> **Version note**: This skill targets Cosmos 1.11+ and Airflow 3.x. If the user is on Airflow 2.x, adjust imports accordingly (see Appendix A).
>
> **Reference**: Latest stable: https://pypi.org/project/astronomer-cosmos/

> **Before starting**, confirm: (1) dbt engine = Core (not Fusion → use **cosmos-dbt-fusion**), (2) warehouse type, (3) Airflow version, (4) execution environment (Airflow env / venv / container), (5) DbtDag vs DbtTaskGroup vs individual operators, (6) manifest availability.

---

## 1. Configure Project (ProjectConfig)

| Approach | When to use | Required param |
|----------|-------------|----------------|
| Project path | Files available locally | `dbt_project_path` |
| Manifest only | `dbt_manifest` load | `manifest_path` + `pro
```

</details>
