---
name: thewiredbear__Claude_Code_Driver__create-skill
source: https://github.com/thewiredbear/Claude_Code_Driver/blob/37a8fdf9d40ce85a0d8328832ba2671f13c76ac5/skills/create_skill.md
repo: thewiredbear/Claude_Code_Driver
kind: skill
stars: 8
last_pushed: 2026-01-28T12:47:48Z
license: mit
score: 9
domains: [agents-ai, cli-tools, dev-ops]
tags: [meta-skill, scaffolding, template]
curated: 2026-06-15
curated_by: config-scout
---

# thewiredbear/Claude_Code_Driver — skill

**Why it's worth keeping:** The heuristic-driven directory analysis (scripts vs. references vs. assets) is a highly transferable pattern for managing complex agent context. It also enforces 'progressive disclosure,' which is critical for preventing token bloat in large skillsets.

**Summary:** A meta-skill that scaffolds structured Claude skills with validated YAML frontmatter and intelligent sub-directory organization.

**Source credibility:** 8 stars suggests a niche but effective utility developed by an active contributor.

**Recency:** Current; aligned with the latest Claude Code skill-based architecture.

**Source:** [thewiredbear/Claude_Code_Driver/skills/create_skill.md](https://github.com/thewiredbear/Claude_Code_Driver/blob/37a8fdf9d40ce85a0d8328832ba2671f13c76ac5/skills/create_skill.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
Slash command to generate new Claude Skills with proper structure, YAML frontmatter, and bundled resources

💡 Use Case: Use when creating reusable skills for workflows, file operations, or specialized tasks that Claude can invoke automatically


---

description: Generate a new Claude Skill with proper structure and YAML frontmatter using official documentation as reference
argument-hint: [skill-name] [description]

---

## /create-skill

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
   - If user provides additional fron
```

</details>
