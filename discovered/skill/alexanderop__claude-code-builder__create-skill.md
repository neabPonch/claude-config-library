---
name: alexanderop__claude-code-builder__create-skill
source: https://github.com/alexanderop/claude-code-builder/blob/85375792c7cac084966e9058a204b94e4f0a638d/commands/create-skill.md
repo: alexanderop/claude-code-builder
kind: skill
stars: 35
last_pushed: 2025-11-16T12:37:57Z
license: mit
score: 9
domains: [agents-ai, cli-tools]
tags: [scaffolding, meta-skill, automation]
curated: 2026-06-15
curated_by: config-scout
---

# alexanderop/claude-code-builder — skill

**Why it's worth keeping:** It implements a 'Progressive Disclosure' pattern to prevent context bloat and includes intelligent logic for bundling scripts, references, and assets based on skill intent.

**Summary:** A meta-skill that automates the scaffolding of new Claude Skills with consistent directory structures and documentation templates.

**Source credibility:** Niche utility; 35 stars indicates a specialized tool rather than a widely-vetted industry standard.

**Recency:** Current; aligns with the architectural requirements of modern Claude Code skills.

**Source:** [alexanderop/claude-code-builder/commands/create-skill.md](https://github.com/alexanderop/claude-code-builder/blob/85375792c7cac084966e9058a204b94e4f0a638d/commands/create-skill.md) · 35★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
description: Generate a new Claude Skill with proper structure and YAML frontmatter using official documentation as reference
argument-hint: [skill-name] [description]
---

# /create-skill

## Purpose
Generate a new Claude Skill with proper structure and YAML frontmatter using official documentation as reference

## Contract
**Inputs:**
- `$1` — SKILL_NAME (lowercase, kebab-case, max 64 characters)
- `$2` — DESCRIPTION (what the skill does and when to use it, max 1024 characters)
- `--personal` — create in ~/.claude/skills/ (default)
- `--project` — create in .claude/skills/

**Outputs:** `STATUS=<CREATED|EXISTS|FAIL> PATH=<path>`

## Instructions

1. **Validate inputs:**
   - Skill name: lowercase letters, numbers, hyphens only (max 64 chars)
   - Description: non-empty, max 1024 characters, no angle brackets (< or >)
   - Description should include both WHAT the skill does and WHEN to use it
   - If user provides additional frontmatter properties, validate against allowed list:
     - **Allowed:** name, description, license, allowed-tools, metadata
     - **Warning** (not error) for unexpected properties like version, author, tags
     - Inform user that unexpected properties
```

</details>
