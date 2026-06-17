---
name: steverozen__clockify-skill
source: https://github.com/steverozen/clockify-skill/blob/69e46224f50b42b2d71009dc5ff7d65db1add97b/skill.md
repo: steverozen/clockify-skill
kind: skill
stars: 0
last_pushed: 2026-04-20T17:06:37Z
license: mit
score: 8
domains: [cli-tools, productivity, api-wrappers]
tags: [time-tracking, python-cli, automation]
curated: 2026-06-14
curated_by: config-scout
---

# steverozen/clockify-skill — skill

**Why it's worth keeping:** The 'Process' section defines high-quality decision trees for error recovery (e.g., running 'ls' when matches are ambiguous). It also demonstrates how to use quoted shell globs to bridge natural language with fuzzy CLI searching.

**Summary:** Provides a sophisticated wrapper for a local Python CLI to manage Clockify time tracking. It includes logic for ambiguity resolution and handling specific CLI warning states.

**Source credibility:** Low star count, but the documentation quality suggests a highly functional, specialized personal tool.

**Recency:** Current; follows modern skill file patterns including versioning and user-invocable flags.

**Source:** [steverozen/clockify-skill/skill.md](https://github.com/steverozen/clockify-skill/blob/69e46224f50b42b2d71009dc5ff7d65db1add97b/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: clockify
description: Clockify time tracking. Start/stop/list timers via natural language. Wraps the colocated `clockify.py` CLI; uses case-insensitive globs to match clients and projects.
version: 0.1.2
user_invocable: true
---

# Clockify Time Tracking

> **Alpha (v0.1.2).** Behavior and flags may change. Verify start/stop times
> in the Clockify UI before trusting them for billing.

## When to Use
Any time the user mentions time tracking, timers, billable time, or names a client/project in a "start working on X" / "stop" / "what's running" / "list projects" context. Examples:

- "start a timer for <client> <project>"
- "stop the timer"
- "I'm working on <project> now"
- "list projects for <client>"
- "what clients do I have matching <glob>?"

## Invoking the CLI

The `clockify.py` script ships in the same folder as this `skill.md`. **Do not rely on `$PATH`.** Invoke it by its absolute path. The canonical install location for a user-scoped skill is:

```bash
python3 ~/.claude/skills/clockify/clockify.py <subcommand> [args]
```

If installed elsewhere (e.g. a project-scoped `.claude/skills/clockify/`, or a different user-level path), substitute that directory. The script
```

</details>
