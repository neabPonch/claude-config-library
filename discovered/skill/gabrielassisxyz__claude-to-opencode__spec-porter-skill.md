---
name: gabrielassisxyz__claude-to-opencode__spec-porter-skill
source: https://github.com/gabrielassisxyz/claude-to-opencode/blob/d2b09240823e66a7c8d07b2f4bb4a8206c21c028/docs/spec-porter-skill.md
repo: gabrielassisxyz/claude-to-opencode
kind: skill
stars: 0
last_pushed: 2026-05-06T01:40:47Z
license: unknown
score: 8
domains: [agents-ai, cli-tools, devops]
tags: [migration, automation, agent-config]
curated: 2026-06-16
curated_by: config-scout
---

# gabrielassisxyz/claude-to-opencode — skill

**Why it's worth keeping:** Includes highly transferable heuristics for inferring model temperature from description text and mapping tool access to security permission postures (allow vs ask).

**Summary:** A technical specification for a migration tool that automates the translation of AI agent configurations between different schema formats.

**Source credibility:** Low visibility/stars, but demonstrates high-level architectural thinking regarding agent configuration.

**Recency:** Extremely current; updated within the last month.

**Source:** [gabrielassisxyz/claude-to-opencode/docs/spec-porter-skill.md](https://github.com/gabrielassisxyz/claude-to-opencode/blob/d2b09240823e66a7c8d07b2f4bb4a8206c21c028/docs/spec-porter-skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
title: "Technical Spec — Porter Skill"
type: spec
created: 2026-05-05
updated: 2026-05-05
status: draft
tags: [spec, opencode, claude-code, porting, skill-architecture]
aliases: [porter-spec, porter-technical-spec]
related:
  - "[[prd-claude-to-opencode-porter]]"
---

# Technical Spec — Porter Skill

## Skill Definition

```
skills/
└── porter/
    ├── SKILL.md              # Main skill file
    ├── scripts/
    │   ├── parse-frontmatter.sh    # Extract YAML from markdown
    │   ├── validate-output.sh      # Lint generated files
    │   └── detect-source-type.sh   # Classify input files
    └── references/
        ├── tool-mapping.md         # Canonical tool translation table
        ├── permission-templates.md # Default permission blocks
        └── opencode-schema.md      # Target format reference
```

## SKILL.md Content

```yaml
---
name: porter
description: Port Claude Code skills, agents, and commands to OpenCode format. Translates frontmatter schemas, maps tool declarations to boolean flags, infers zero-trust permissions, assigns temperature and mode, generates companion command files. Trigger when user mentions porting, migrating, or converting between Claude Code and
```

</details>
