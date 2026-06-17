---
name: astronomer__astronomer__skill
source: https://github.com/astronomer/astronomer/blob/97394661f9efc8ef036983cebbfbb42c84cc4341/.agents/skills/circleci/SKILL.md
repo: astronomer/astronomer
kind: skill
stars: 490
last_pushed: 2026-06-12T15:17:25Z
license: other
score: 8
domains: [devops, ci-cd]
tags: [circleci, jinja2, automation, infrastructure]
curated: 2026-06-15
curated_by: config-scout
---

# astronomer/astronomer — skill

**Why it's worth keeping:** It prevents an AI agent from breaking the build by explicitly documenting that `.circleci/config.yml` is a generated file that must be modified via Jinja2 templates instead.

**Summary:** Enforces strict protocols for CircleCI configuration by mandating script externalization to `bin/` and a template-driven generation workflow.

**Source credibility:** High; Astronomer is an established enterprise platform for Airflow on Kubernetes.

**Recency:** Very current, with active repository maintenance reported within the last month.

**Source:** [astronomer/astronomer/.agents/skills/circleci/SKILL.md](https://github.com/astronomer/astronomer/blob/97394661f9efc8ef036983cebbfbb42c84cc4341/.agents/skills/circleci/SKILL.md) · 490★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: circleci
description: Use when writing, editing, or reviewing CircleCI configuration for the Astronomer APC repository. Covers script organization, inline vs external scripts, and config conventions.
---

# CircleCI Configuration Guide

## Critical Rules

1. **No long inline scripts** — script logic for any language must not be written inline in `.circleci/config.yml` if the script has complicated flow control. Complicated scripts belong in `bin/`.
2. **Scripts live in `bin/`** — every script called from CircleCI must exist as a file in the `bin/` directory with an appropriate extension (e.g. `bin/my-script.sh`, `bin/my-script.py`).
3. **Pin all versions** — never use `latest` or unpinned tags for Docker images or installed tools. Always specify an exact version to prevent supply chain vulnerabilities and ensure reproducible builds.

---

## Script Organization

Scripts invoked by CircleCI jobs must be committed to the repository under `bin/` so they can be:

- Linted and reviewed like any other source file
- Tested and run locally without needing CI
- Reused across multiple jobs or workflows

```yaml
# ✅ CORRECT — call a script from bin/
steps:
  - run:
      name: Build
```

</details>
