---
name: MacHu-GWU__cookiecutter-pywf_open_source
source: https://github.com/MacHu-GWU/cookiecutter-pywf_open_source/blob/f7c9ea9b9bf3517cbc431936dbbe9be777fe082b/CLAUDE.md
repo: MacHu-GWU/cookiecutter-pywf_open_source
kind: claude-md
stars: 2
last_pushed: 2026-04-21T21:10:14Z
license: mit
score: 8
domains: [devops, python, automation]
tags: [cookiecutter, template-generation, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# MacHu-GWU/cookiecutter-pywf_open_source — claude-md

**Why it's worth keeping:** It establishes a clear 'source of truth' rule (change seed, not template) and defines specific automated validation scripts that an AI agent can use to verify its own work.

**Summary:** Documents a high-stakes, 5-step 'reverse engineering' workflow used to maintain a cookiecutter template via a seed project. It provides rigorous verification steps and strict rules to prevent manual errors in the template directory.

**Source credibility:** Low star count, but highly structured and professional-grade automation logic.

**Recency:** Very current, utilizing modern toolchains like mise and uv.

**Source:** [MacHu-GWU/cookiecutter-pywf_open_source/CLAUDE.md](https://github.com/MacHu-GWU/cookiecutter-pywf_open_source/blob/f7c9ea9b9bf3517cbc431936dbbe9be777fe082b/CLAUDE.md) · 2★

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
