---
name: androidx__androidx__skill
source: https://github.com/androidx/androidx/blob/4bad70d4fa5dfa08ada51331507f8657db991963/.agents/skills/api_review/SKILL.md
repo: androidx/androidx
kind: skill
stars: 6009
last_pushed: 2026-06-15T19:40:56Z
license: apache-2.0
score: 8
domains: [android, api-design, mobile-development]
tags: [api-compliance, gradle, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# androidx/androidx — skill

**Why it's worth keeping:** It demonstrates a perfect 'Check-Verify-Report' loop, showing how to integrate exact CLI commands and specific documentation paths into an agent workflow.

**Summary:** This skill automates the validation of API design changes by combining specific Gradle task execution with rigorous guideline compliance checks.

**Source credibility:** Extremely high; the source is an official Google-maintained Android project.

**Recency:** Current; follows modern Gradle/Git workflows used in professional software engineering.

**Source:** [androidx/androidx/.agents/skills/api_review/SKILL.md](https://github.com/androidx/androidx/blob/4bad70d4fa5dfa08ada51331507f8657db991963/.agents/skills/api_review/SKILL.md) · 6009★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: api_review
description: A skill to review pending work for API design compliance in the
AndroidX support project
---

# API Review Skill

This skill provides instructions for evaluating pending work (e.g., a local git
branch or CL) to ensure that any new or modified Public APIs comply with
AndroidX/Jetpack API guidelines.

## Steps for API Review

When the user asks for their pending work to be reviewed for API design, follow
these steps:

### 1. Update and Review API Files (`updateApi`)

First, run the `updateApi` task to ensure all recent changes are accurately
reflected in the API tracking files (e.g., `current.txt` or
`restricted_current.txt`). This catches any new modifications that haven't been
tracked yet.

*   **For all modules:**
    ```bash
    ./gradlew updateApi
    ```
*   **For a single module:** (e.g., `appcompat-resources` in the `appcompat`
    group)
    ```bash
    ./gradlew :appcompat:appcompat-resources:updateApi
    ```
*   **For Compose modules (Kotlin Multiplatform):** Compose is a multiplatform
    project. If you modify APIs that affect native targets (e.g., iOS or
    Desktop), you may also need to update the native ABI files:
    ```bash
    ./
```

</details>
