---
name: nth5693__gemini-kit__skill
source: https://github.com/nth5693/gemini-kit/blob/f3db206869f6f98b43c1207836a51f425527b763/skills/file-todos/SKILL.md
repo: nth5693/gemini-kit
kind: skill
stars: 353
last_pushed: 2026-03-07T12:21:24Z
license: mit
score: 7
domains: [cli-tools, workflow-management]
tags: [task-tracking, state-management, structured-logs]
curated: 2026-06-15
curated_by: config-scout
---

# nth5693/gemini-kit — skill

**Why it's worth keeping:** The rigid filename pattern makes project state highly discoverable via standard filesystem commands. It provides a lightweight, local way for agents to track progress and blockers without needing an external database.

**Summary:** A structured task-tracking system using markdown files with strict naming conventions and YAML frontmatter for dependency management.

**Source credibility:** 353 stars suggests this is a popular and vetted utility kit.

**Recency:** Highly relevant; provides a blueprint for persistent state management in long-running agentic sessions.

**Source:** [nth5693/gemini-kit/skills/file-todos/SKILL.md](https://github.com/nth5693/gemini-kit/blob/f3db206869f6f98b43c1207836a51f425527b763/skills/file-todos/SKILL.md) · 353★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: file-todos
description: Manage file-based todo tracking in the todos/ directory
---

# File-Based Todo Tracking

Provides workflows for creating, managing, and completing todos stored as markdown files.

## Overview

The `todos/` directory contains markdown files with YAML frontmatter for tracking work items.

## File Naming Convention

```
{issue_id}-{status}-{priority}-{description}.md

Examples:
001-pending-p1-security-fix.md
002-ready-p2-performance-opt.md
003-complete-p3-cleanup.md
```

## Status Lifecycle

```
pending → ready → complete
   ↓
(deleted if skipped)
```

## What do you want to do?

1. **Create a todo** → See "Creating Todos" below
2. **Triage pending items** → Use `/triage`
3. **Work on todos** → Use `/resolve_todo`
4. **Check dependencies** → See "Dependency Management" below

---

## Instrumentation

```bash
# Log usage when using this skill
./scripts/log-skill.sh "file-todos" "manual" "$$"
```

## Creating Todos

```bash
# Get next ID
next_id=$(ls todos/*.md 2>/dev/null | grep -o '[0-9]\+' | sort -n | tail -1 | awk '{printf "%03d", $1+1}')
[ -z "$next_id" ] && next_id="001"

# Copy template
cp todos/todo-template.md todos/${next_id}-pending-{priority
```

</details>
