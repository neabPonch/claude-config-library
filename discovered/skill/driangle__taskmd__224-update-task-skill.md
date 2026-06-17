---
name: driangle__taskmd__224-update-task-skill
source: https://github.com/driangle/taskmd/blob/b2f7c29aba7716fdd2b8d24efea0eabb844a0ca4/tasks/224-update-task-skill.md
repo: driangle/taskmd
kind: skill
stars: 41
last_pushed: 2026-04-23T16:12:24Z
license: mit
score: 8
domains: [agents-ai, cli-tools, task-management]
tags: [template, workflow-orchestration, structured-planning]
curated: 2026-06-15
curated_by: config-scout
---

# driangle/taskmd — skill

**Why it's worth keeping:** It defines high-level logic for tool usage (CLI vs. direct file editing) and uses explicit Acceptance Criteria to prevent scope creep or hallucinations.

**Summary:** A rigorous task-definition template using frontmatter and hierarchical checklists to drive agentic workflows.

**Source credibility:** Niche repository with recent, highly structured development.

**Recency:** Extremely current/future-dated, aligning with advanced agentic planning requirements.

**Source:** [driangle/taskmd/tasks/224-update-task-skill.md](https://github.com/driangle/taskmd/blob/b2f7c29aba7716fdd2b8d24efea0eabb844a0ca4/tasks/224-update-task-skill.md) · 41★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
title: "Add update-task skill to plugin"
id: "224"
status: completed
priority: medium
type: feature
tags: []
created: "2026-02-26"
---

# Add update-task skill to plugin

## Objective

Add a new "update-task" skill to the Claude Code plugin (`claude-code-plugin/skills/`) that allows users to update an existing task's fields (status, priority, title, tags, dependencies, etc.) via a natural language command. This complements the existing `get-task`, `add-task`, `complete-task`, and `set` CLI functionality.

## Tasks

- [x] Create `claude-code-plugin/skills/update-task/` directory with skill definition
- [x] Define the skill prompt that parses user intent and determines which fields to update
- [x] For CLI-supported fields (status, priority, effort, tags, owner, parent, type, PRs), instruct the agent to use `taskmd set` with appropriate flags
- [x] For fields not supported by `taskmd set` (title, dependencies, custom frontmatter), instruct the agent to edit the task file directly
- [x] Document which fields use CLI vs direct file editing in the skill prompt
- [x] Register the skill in the plugin manifest
- [x] Handle edge cases (invalid IDs, invalid field values) with clear error
```

</details>
