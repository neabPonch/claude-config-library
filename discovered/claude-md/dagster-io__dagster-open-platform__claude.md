---
name: dagster-io__dagster-open-platform__claude
source: https://github.com/dagster-io/dagster-open-platform/blob/dc5e7b4bb3873c4120a6f92f7960531291bef3f7/dagster_open_platform_dbt/CLAUDE.md
repo: dagster-io/dagster-open-platform
kind: claude-md
stars: 463
last_pushed: 2026-06-11T00:09:40Z
license: unknown
score: 8
domains: [data-engineering, analytics]
tags: [dbt, architecture, guardrails]
curated: 2026-06-16
curated_by: config-scout
---

# dagster-io/dagster-open-platform — claude-md

**Why it's worth keeping:** It provides high-value architectural guardrails, such as explicit 'Restricted Areas' to prevent legacy code pollution and instructions on maintaining YAML/schema synchronization.

**Summary:** Defines a multi-layer dbt transformation architecture with strict rules for how data moves between stages.

**Source credibility:** High; authored by Dagster Labs, a major player in the data orchestration space.

**Recency:** Current; focuses on structural constraints that are highly effective for modern AI coding agents.

**Source:** [dagster-io/dagster-open-platform/dagster_open_platform_dbt/CLAUDE.md](https://github.com/dagster-io/dagster-open-platform/blob/dc5e7b4bb3873c4120a6f92f7960531291bef3f7/dagster_open_platform_dbt/CLAUDE.md) · 463★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# DBT Project Overview

This document outlines the structure, purpose, and best practices for our dbt project.
It is intended for LLM-assisted documentation, query generation, and analytics support.

---

## 1. Staging Layer
- **Purpose:** Add brand new raw data.
- **Organization:** Subdirectories per data source (e.g., Google Search Console, LinkedIn Ads, Salesforce, Reddit Ads, etc.).
- **Processing:**
  - Minimal transformations.
  - Primarily **renaming fields**.
  - No additional logic applied at this stage.
- **Best Practice:** Before creating a new file, **check if one already exists** to avoid duplication.

---

## 2. Models Layer
- **Purpose:** Add context and reusable logic.
- **Characteristics:** Generally a **one-to-one relationship** with the staging layer.
- **Processing:**
  - Add **case statements** and other reusable logic.
  - Apply **filters** to exclude unnecessary data.
- **Output:** Feeds into the **core layer**.
- **Best Practice:** Before creating a new file, **check if one already exists** to avoid duplication.

---

## 3. Core Layer
- **Purpose:** Create **dimension and fact tables**.
- **Processing:**
  - Consolidates and standardizes data.
  - Enables re
```

</details>
