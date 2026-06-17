---
name: foryourhealth111-pixel__Vibe-Skills__skill
source: https://github.com/foryourhealth111-pixel/Vibe-Skills/blob/25ab877ad0e2b0631c28399772941b9f35401b0b/bundled/skills/speckit-implement/SKILL.md
repo: foryourhealth111-pixel/Vibe-Skills
kind: skill
stars: 2307
last_pushed: 2026-05-19T15:42:16Z
license: apache-2.0
score: 8
domains: [cli-tools, software-engineering, devops]
tags: [orchestration, tdd, task-management]
curated: 2026-06-16
curated_by: config-scout
---

# foryourhealth111-pixel/Vibe-Skills — skill

**Why it's worth keeping:** The fail-safe checklist verification prevents execution if planning is incomplete, and the proactive '.ignore' file detection logic provides excellent environment hygiene.

**Summary:** A high-level orchestration skill that enforces a rigorous TDD workflow by checking plan completion before starting implementation.

**Source credibility:** Highly credible; high star count and recent updates suggest a robust toolset.

**Recency:** Current; includes modern technology patterns like Docker, ESM/Node, and various language-specific ignore patterns.

**Source:** [foryourhealth111-pixel/Vibe-Skills/bundled/skills/speckit-implement/SKILL.md](https://github.com/foryourhealth111-pixel/Vibe-Skills/blob/25ab877ad0e2b0631c28399772941b9f35401b0b/bundled/skills/speckit-implement/SKILL.md) · 2307★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: speckit-implement
description: Execute all tasks from the task breakdown to build the feature. Use after
  task generation to systematically implement the planned solution following TDD approach
  where applicable.
compatibility: Requires spec-kit project structure with .specify/ directory
metadata:
  author: github-spec-kit
  source: templates/commands/implement.md
---

# Speckit Implement Skill

## User Input

```text
$ARGUMENTS
```

You **MUST** consider the user input before proceeding (if not empty).

## Outline

1. Run `.specify/scripts/powershell/check-prerequisites.ps1 -Json -RequireTasks -IncludeTasks` from repo root and parse FEATURE_DIR and AVAILABLE_DOCS list. All paths must be absolute. For single quotes in args like "I'm Groot", use escape syntax: e.g 'I'\''m Groot' (or double-quote if possible: "I'm Groot").

2. **Check checklists status** (if FEATURE_DIR/checklists/ exists):
   - Scan all checklist files in the checklists/ directory
   - For each checklist, count:
     - Total items: All lines matching `- [ ]` or `- [X]` or `- [x]`
     - Completed items: Lines matching `- [X]` or `- [x]`
     - Incomplete items: Lines matching `- [ ]`
   - Create a status
```

</details>
