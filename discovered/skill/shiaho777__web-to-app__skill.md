---
name: shiaho777__web-to-app__skill
source: https://github.com/shiaho777/web-to-app/blob/6067b9571179b7338a0840e0be8231118ceb1f7f/app/src/main/assets/skills/python-app/SKILL.md
repo: shiaho777/web-to-app
kind: skill
stars: 4201
last_pushed: 2026-06-14T17:14:22Z
license: unlicense
score: 8
domains: [backend-api, python]
tags: [environment-constraints, workflow-optimization]
curated: 2026-06-15
curated_by: config-scout
---

# shiaho777/web-to-app — skill

**Why it's worth keeping:** Uses effective negative constraints ('Don'ts') to prevent environment errors and implements a strict communication protocol (one-line summaries + stop) to maintain user control over the development loop.

**Summary:** A highly constrained persona for building Python web applications within a specific sandboxed, on-device runtime.

**Source credibility:** High star count suggests the underlying project is a legitimate, widely-used tool.

**Recency:** Current; uses modern agentic interaction patterns like specific instruction-following and task-oriented pauses.

**Source:** [shiaho777/web-to-app/app/src/main/assets/skills/python-app/SKILL.md](https://github.com/shiaho777/web-to-app/blob/6067b9571179b7338a0840e0be8231118ceb1f7f/app/src/main/assets/skills/python-app/SKILL.md) · 4201★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: python-app
description: Build a Python web app (Flask, Django, or stdlib) on the on-device Python runtime
when_to_use: User wants a Python backend, ML demo, or scripting endpoint
icon: language
icon_color: 3B82F6
category: app
allowed_tools:
  - Read
  - Write
  - Edit
  - Delete
  - Glob
  - Grep
  - ListFiles
  - AskUserQuestion
  - TodoWrite
  - TodoUpdate
arguments: prompt
---

# Python App

You build Python web apps that run on the on-device Python 3.10+ runtime.

## Pick a framework based on scope

- **stdlib `http.server`**: 1-3 endpoints, no deps, no template engine needed.
- **Flask**: 4-20 endpoints, simple templates, modest deps. Default choice.
- **Django**: full admin / ORM / multi-app. Only when the user explicitly asks.

## Constraints

- Listen on `int(os.environ.get('PORT', '8000'))`.
- Use SQLite for persistence (`sqlite3` stdlib module). Other databases require a separate server.
- Native deps (numpy, scikit-learn) work but cold-start is slow. Prefer pure-Python.
- No `subprocess` shell access; the sandbox blocks shell commands.

## File layout (Flask)

```
requirements.txt        ← minimal, pinned versions
app.py                  ← Flask application fa
```

</details>
