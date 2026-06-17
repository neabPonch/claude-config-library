---
name: MacHu-GWU__cookiecutter-aws_lbd
source: https://github.com/MacHu-GWU/cookiecutter-aws_lbd/blob/d2ce2b33ffeab8b185a665318c61054f0575d7cb/CLAUDE.md
repo: MacHu-GWU/cookiecutter-aws_lbd
kind: claude-md
stars: 0
last_pushed: 2026-04-28T17:20:09Z
license: mit
score: 8
domains: [cli-tools, devops, python]
tags: [cookiecutter, automation-workflow, aws-lambda]
curated: 2026-06-16
curated_by: config-scout
---

# MacHu-GWU/cookiecutter-aws_lbd — claude-md

**Why it's worth keeping:** Provides critical procedural guardrails that prevent the AI from editing the template directly and lists exact command sequences for highly specific verification steps.

**Summary:** Documents a specialized 'seed-to-template' workflow where changes must be made in a separate project before being converted into this cookiecutter template.

**Source credibility:** Low star count, but shows high technical sophistication via specialized automation scripts.

**Recency:** Current; utilizes modern toolchains like mise and uv.

**Source:** [MacHu-GWU/cookiecutter-aws_lbd/CLAUDE.md](https://github.com/MacHu-GWU/cookiecutter-aws_lbd/blob/d2ce2b33ffeab8b185a665318c61054f0575d7cb/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

This is a **cookiecutter project template** (`cookiecutter-aws_lbd`) for generating Python open source library projects. It is maintained using a "reverse engineering" approach: a real seed project is converted into a cookiecutter template via an automated script.

- **This repo** (template): `$HOME/GitHub/cookiecutter-aws_lbd`
- **Seed repo** (concrete project): `$HOME/GitHub/cookiecutter_aws_lbd_demo-project`
- **Generated template dir**: `{{ cookiecutter.package_name }}-project/`

## Maintenance Workflow (5-Step Process)

**IMPORTANT:** Always make changes in the **Seed project** first, never edit the template directly.

### Step 1: `mise run make-template`
**Purpose:** Convert the seed project into a cookiecutter template

- Reads the seed project from `$HOME/GitHub/cookiecutter_aws_lbd_demo-project`
- Replaces concrete values (e.g., `cookiecutter_aws_lbd_demo`) with placeholders (e.g., `{{ cookiecutter.package_name }}`)
- Outputs the generated template to `tmp/` directory
- Script: `.mise/tasks/make_template.py`

**What to do:** Review the generated template in `tmp/` to ensure it looks correct.

### Step 2: `mise run check-seed-values`
**Purp
```

</details>
