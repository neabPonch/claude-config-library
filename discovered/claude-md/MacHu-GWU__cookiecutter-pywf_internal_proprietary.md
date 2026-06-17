---
name: MacHu-GWU__cookiecutter-pywf_internal_proprietary
source: https://github.com/MacHu-GWU/cookiecutter-pywf_internal_proprietary/blob/2b414af42d7cf6ed6fcdc633494af3fb6be599d7/CLAUDE.md
repo: MacHu-GWU/cookiecutter-pywf_internal_proprietary
kind: claude-md
stars: 0
last_pushed: 2026-04-15T17:29:21Z
license: mit
score: 8
domains: [cli-tools, devops, templating]
tags: [python, cookiecutter, workflow-automation]
curated: 2026-06-16
curated_by: config-scout
---

# MacHu-GWU/cookiecutter-pywf_internal_proprietary — claude-md

**Why it's worth keeping:** The multi-step verification process (checking for leaked seed values and unresolved placeholders) is a perfect pattern for instructing AI on complex meta-programming/templating tasks.

**Summary:** This file documents a high-integrity 'seed-to-template' workflow that uses automated validation steps to ensure template correctness.

**Source credibility:** Low social proof (0 stars), but highly detailed technical documentation suggests a specialized internal tool.

**Recency:** 

**Source:** [MacHu-GWU/cookiecutter-pywf_internal_proprietary/CLAUDE.md](https://github.com/MacHu-GWU/cookiecutter-pywf_internal_proprietary/blob/2b414af42d7cf6ed6fcdc633494af3fb6be599d7/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

This is a **cookiecutter project template** (`cookiecutter-pywf_open_source`) for generating Python open source library projects. It is maintained using a "reverse engineering" approach: a real seed project is converted into a cookiecutter template via an automated script.

- **This repo** (template): `$HOME/GitHub/cookiecutter-pywf_open_source`
- **Seed repo** (concrete project): `$HOME/GitHub/cookiecutter_pywf_open_source_demo-project`
- **Generated template dir**: `{{ cookiecutter.package_name }}-project/`

## Maintenance Workflow (5-Step Process)

**IMPORTANT:** Always make changes in the **Seed project** first, never edit the template directly.

### Step 1: `mise run make-template`
**Purpose:** Convert the seed project into a cookiecutter template

- Reads the seed project from `$HOME/GitHub/cookiecutter_pywf_open_source_demo-project`
- Replaces concrete values (e.g., `cookiecutter_pywf_open_source_demo`) with placeholders (e.g., `{{ cookiecutter.package_name }}`)
- Outputs the generated template to `tmp/` directory
- Script: `.mise/tasks/make_template.py`

**What to do:** Review the generated template in `tmp/` to ensure it looks correct.

##
```

</details>
