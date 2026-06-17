---
name: OpenHands__extensions__skill
source: https://github.com/OpenHands/extensions/blob/e15748cf0e13dccb73fef1a403a4b2e6212fdc46/skills/spark-version-upgrade/SKILL.md
repo: OpenHands/extensions
kind: skill
stars: 114
last_pushed: 2026-06-15T17:47:32Z
license: mit
score: 9
domains: [data-engineering, devops]
tags: [spark, migration, upgrade]
curated: 2026-06-15
curated_by: config-scout
---

# OpenHands/extensions — skill

**Why it's worth keeping:** It provides specific shell commands (grep) for impact analysis and emphasizes behavioral logic shifts in SQL/DataFrame that are often overlooked during version bumps.

**Summary:** A comprehensive, phase-based workflow for migrating Apache Spark applications across major versions including API and configuration changes.

**Source credibility:** High; part of the OpenHands repository, a reputable open-source autonomous software engineering project.

**Recency:** Current; covers modern Spark versions including 3.x to 4.x transitions.

**Source:** [OpenHands/extensions/skills/spark-version-upgrade/SKILL.md](https://github.com/OpenHands/extensions/blob/e15748cf0e13dccb73fef1a403a4b2e6212fdc46/skills/spark-version-upgrade/SKILL.md) · 114★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: spark-version-upgrade
description: Upgrade Apache Spark applications between major versions (2.x→3.x, 3.x→4.x). Covers build files, deprecated APIs, configuration changes, SQL/DataFrame updates, and test validation.
license: MIT
compatibility: Requires Java 8+/11+/17+, Scala 2.12/2.13, Maven/Gradle/SBT, Apache Spark
triggers:
  - spark upgrade
  - spark migration
  - spark version
  - upgrade spark
  - spark 3
  - spark 4
  - pyspark upgrade
---

Upgrade Apache Spark applications between major versions with a structured, phase-by-phase workflow.

## When to Use

- Migrating from Spark 2.x → 3.x or Spark 3.x → 4.x
- Updating PySpark, Spark SQL, or Structured Streaming applications
- Resolving deprecation warnings before a Spark version bump

## Workflow Overview

1. **Inventory & Impact Analysis** — Scan the codebase and assess scope
2. **Build File Updates** — Bump Spark/Scala/Java dependencies
3. **API Migration** — Replace deprecated and removed APIs
4. **Configuration Migration** — Update Spark config properties
5. **SQL & DataFrame Migration** — Fix query-level breaking changes
6. **Test Validation** — Compile, run tests, verify results

---

## Phase 1: Inventory & I
```

</details>
