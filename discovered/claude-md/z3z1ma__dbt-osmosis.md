---
name: z3z1ma__dbt-osmosis
source: https://github.com/z3z1ma/dbt-osmosis/blob/39942c69985ecfda8e9d8bc48b3c9ec57a56eefa/CLAUDE.md
repo: z3z1ma/dbt-osmosis
kind: claude-md
stars: 630
last_pushed: 2026-06-13T19:33:00Z
license: apache-2.0
score: 9
domains: [cli-tools, data-engineering, python]
tags: [workflow-driven, architecture-mapping, command-reference]
curated: 2026-06-15
curated_by: config-scout
---

# z3z1ma/dbt-osmosis — claude-md

**Why it's worth keeping:** The inclusion of a specialized task-based workflow (beads) and the explanation of 'logical pipelines' instead of just a file tree are top-tier techniques. It also defines complex configuration precedence rules which prevents AI-generated errors in logic.

**Summary:** This file provides comprehensive operational instructions including specific issue-tracking workflows, detailed command sets for dev/test cycles, and deep architectural logic explanations.

**Source credibility:** High: active maintenance, significant star count, and high-quality toolchain usage (uv/task).

**Recency:** 

**Source:** [z3z1ma/dbt-osmosis/CLAUDE.md](https://github.com/z3z1ma/dbt-osmosis/blob/39942c69985ecfda8e9d8bc48b3c9ec57a56eefa/CLAUDE.md) · 630★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Issue Tracking

This project uses **bd (beads)** for issue tracking.
Run `bd prime` for workflow context, or install hooks (`bd hooks install`) for auto-injection.

**Quick reference:**
- `bd ready` - Find unblocked work
- `bd create "Title" --type task --priority 2` - Create issue
- `bd close <id>` - Complete work
- `bd sync` - Sync with git (run at session end)

For full workflow details: `bd prime`

## Repository Overview

**dbt-osmosis** is a CLI tool that enhances the dbt developer experience through automated YAML schema management, column-level documentation inheritance, and a Streamlit-based workbench for interactive dbt SQL development. The tool operates as both a dbt utility and standalone Python package.

## Development Commands

### Environment Setup
```bash
# Install task runner (see https://taskfile.dev/installation/)
# Then run default task (format, lint, dev setup, test)
task

# Setup dev environment only
task dev

# Create virtual environment
task venv
```

### Code Quality
```bash
# Format code (auto-fix imports + ruff format)
task format

# Lint code
task lint

# Manual ruff commands
uvx ruff check
uvx ruff format --preview
uvx ruff check --fix --
```

</details>
