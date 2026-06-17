---
name: ClawBio__ClawBio__skill
source: https://github.com/ClawBio/ClawBio/blob/2267e1fc8129cf527edfb3ffc68042512121ca13/skills/skill-builder/SKILL.md
repo: ClawBio/ClawBio
kind: skill
stars: 970
last_pushed: 2026-06-14T19:30:59Z
license: mit
score: 9
domains: [bioinformatics, cli-tools, meta-programming, agents-ai]
tags: [scaffolding, automation, dev-ops]
curated: 2026-06-15
curated_by: config-scout
---

# ClawBio/ClawBio — skill

**Why it's worth keeping:** The 'Algorithm / Methodology' section provides a clear execution plan for complex multi-step tasks; the use of formal specs (JSON) to drive generation is a top-tier pattern for reliability.

**Summary:** A meta-skill designed to scaffold new, highly structured AI agent skills using JSON/YAML specifications or interactive prompts. It automates the creation of documentation, Python skeletons, test suites, and registry updates.

**Source credibility:** High; high star count and active, recent development in the bioinformatics domain.

**Recency:** Very current, utilizing modern Python standards and sophisticated agentic workflows.

**Source:** [ClawBio/ClawBio/skills/skill-builder/SKILL.md](https://github.com/ClawBio/ClawBio/blob/2267e1fc8129cf527edfb3ffc68042512121ca13/skills/skill-builder/SKILL.md) · 970★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: skill-builder
description: Scaffold a new ClawBio skill from a spec file (JSON/YAML) or interactively — generates SKILL.md, Python skeleton, tests, and updates catalog.json
version: 0.1.0
author: Mj
license: MIT
tags: [meta, scaffolding, developer-tools, skill-creation]
metadata:
  openclaw:
    requires:
      bins:
        - python3
      env: []
      config: []
    always: false
    emoji: "🦖"
    homepage: https://github.com/ClawBio/ClawBio
    os: [darwin, linux]
    install: []
    trigger_keywords:
      - create skill
      - new skill
      - scaffold skill
      - skill template
      - skill builder
      - add a skill
      - build a skill
      - make a skill
---

# 🦖 Skill Builder

You are **Skill Builder**, a specialised ClawBio meta-skill for scaffolding new skills. Your role is to take a skill specification and generate a complete, PR-ready ClawBio skill directory with all required files.

## Why This Exists

- **Without it**: Contributors must manually copy the template, fill in every section, write a Python skeleton from scratch, and manually update `catalog.json` and `clawbio.py` — a 30-60 minute process prone to missing required sections or malformed
```

</details>
