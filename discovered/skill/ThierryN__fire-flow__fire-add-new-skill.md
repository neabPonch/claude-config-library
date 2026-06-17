---
name: ThierryN__fire-flow__fire-add-new-skill
source: https://github.com/ThierryN/fire-flow/blob/c67b9f4b819e8efb58f0a16b67782722408d0b83/commands/fire-add-new-skill.md
repo: ThierryN/fire-flow
kind: skill
stars: 75
last_pushed: 2026-03-26T04:04:33Z
license: mit
score: 9
domains: [agents-ai, developer-experience, cli-tools, knowledge-management]
tags: [skill-extraction, wizard, pattern-capture, meta-programming]
curated: 2026-06-15
curated_by: config-scout
---

# ThierryN/fire-flow — skill

**Why it's worth keeping:** The use of Mermaid diagrams to enforce step-by-step agent adherence and the distinction between 'General' vs 'Project' scope are highly sophisticated patterns for managing AI memory.

**Summary:** An interactive 'knowledge capture' wizard that extracts technical solutions from current sessions or logs and organizes them into a structured skill library.

**Source credibility:** High; the repo has significant stars (75) and recent maintenance, indicating a high-quality orchestration framework.

**Recency:** Current; specifically designed to leverage Claude Code's file-reading and session context capabilities.

**Source:** [ThierryN/fire-flow/commands/fire-add-new-skill.md](https://github.com/ThierryN/fire-flow/blob/c67b9f4b819e8efb58f0a16b67782722408d0b83/commands/fire-add-new-skill.md) · 75★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: power-add-new-skill
description: Add a new skill to the skills library when you solve a hard problem
arguments:
  - name: from
    description: Source for skill extraction (summary, session, or manual)
    required: false
    type: string
    default: "interactive"
triggers:
  - "add skill"
  - "contribute skill"
  - "new skill"
  - "save pattern"
---

# /fire-add-new-skill - Add New Skill to Library

Interactive wizard to contribute new skills to the Dominion Flow skills library.

## Purpose

Capture and preserve proven solutions when you:
- Solve a challenging technical problem
- Discover a reusable pattern
- Find a better approach than existing skills
- Want to share knowledge across projects

## Arguments

| Argument | Required | Description |
|----------|----------|-------------|
| `from` | No | Source: `summary` (from RECORD.md), `session` (current work), `manual` (interactive) |

## Usage Examples

```bash
# Interactive wizard (default)
/fire-add-new-skill

# Extract from most recent RECORD.md
/fire-add-new-skill --from summary

# Extract from current session context
/fire-add-new-skill --from session

# Quick contribute with inline details
/fire-add-new-skill --na
```

</details>
