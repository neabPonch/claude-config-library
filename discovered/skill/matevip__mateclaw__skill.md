---
name: matevip__mateclaw__skill
source: https://github.com/matevip/mateclaw/blob/d9a9d07704e9c49d185eaa8418c870568a74a846/mateclaw-server/src/main/resources/skills/skill-authoring/SKILL.md
repo: matevip/mateclaw
kind: skill
stars: 621
last_pushed: 2026-06-15T08:14:27Z
license: apache-2.0
score: 8
domains: [agents-ai, cli-tools, documentation]
tags: [skill-authoring, meta-instructions, schema]
curated: 2026-06-15
curated_by: config-scout
---

# matevip/mateclaw — skill

**Why it's worth keeping:** It enforces high-reliability patterns like 'When to Use/Don't use for' and mandatory Verification Checklists which reduce agent hallucination and misuse.

**Summary:** Defines a rigorous specification for authoring agent skills using YAML frontmatter and structured Markdown documentation.

**Source credibility:** Strong: 621 stars and very active recent maintenance.

**Recency:** Extremely current, reflecting modern multi-agent orchestration needs.

**Source:** [matevip/mateclaw/mateclaw-server/src/main/resources/skills/skill-authoring/SKILL.md](https://github.com/matevip/mateclaw/blob/d9a9d07704e9c49d185eaa8418c870568a74a846/mateclaw-server/src/main/resources/skills/skill-authoring/SKILL.md) · 621★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: skill-authoring
description: 'Author SKILL.md skills: frontmatter, validator limits, structure.'
version: 1.0.0
tags:
- skills
- authoring
- skill-md
- conventions
- meta
author: ported
---
# Authoring MateClaw Skills

## Overview

A skill is a `SKILL.md` file — YAML frontmatter plus a markdown body of reusable instructions. There are two places a SKILL.md can live, and they have different creation paths:

1. **Builtin (in-repo):** `mateclaw-server/src/main/resources/skills/<name>/SKILL.md` — committed, shipped inside the server JAR. On every startup `BuiltinSkillSeedService` scans `classpath*:skills/*/SKILL.md`, parses each frontmatter, and upserts a row into `mate_skill` keyed by `name`. The SKILL.md is the single source of truth — no SQL seed entry is required.
2. **Custom (runtime):** created by an agent or user through the `skill_manage` tool. Stored as a `mate_skill` row with `skill_type=custom` and exported to the workspace at `~/.mateclaw/skills/<name>/`. Not committed; lives per-installation.

This skill covers both. Note that `skill_manage` does NOT write into the in-repo `skills/` tree — builtin skills are authored by writing the file directly and restarting.
```

</details>
