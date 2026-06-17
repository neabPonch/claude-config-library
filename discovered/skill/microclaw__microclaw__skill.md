---
name: microclaw__microclaw__skill
source: https://github.com/microclaw/microclaw/blob/f179719f7af205ebd49242bb14ac8d693ea23242/skills/built-in/shell-scripting/SKILL.md
repo: microclaw/microclaw
kind: skill
stars: 718
last_pushed: 2026-06-14T06:24:37Z
license: mit
score: 8
domains: [cli-tools, devops]
tags: [shell, bash, scripting, automation]
curated: 2026-06-15
curated_by: config-scout
---

# microclaw/microclaw — skill

**Why it's worth keeping:** Enforces 'set -euo pipefail' for error handling and provides essential patterns like temporary file cleanup using traps and existence checks.

**Summary:** Provides strict, defensive programming standards for generating robust and safe shell scripts.

**Source credibility:** High-quality content from a growing Rust-based agentic assistant project.

**Recency:** Current; uses modern shell scripting best practices.

**Source:** [microclaw/microclaw/skills/built-in/shell-scripting/SKILL.md](https://github.com/microclaw/microclaw/blob/f179719f7af205ebd49242bb14ac8d693ea23242/skills/built-in/shell-scripting/SKILL.md) · 718★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: shell-scripting
description: "Write robust, safe bash/shell scripts and one-liners, and explain or fix existing ones. Use when users want a shell script, a command pipeline, automation glue, or ask why a bash snippet misbehaves (quoting, globbing, exit codes). Triggers on mentions of bash, shell script, .sh, command line, pipe, one-liner, cron job command, 脚本, 命令行, 管道, shell."
license: Proprietary. LICENSE.txt has complete terms
compatibility: "No external dependencies. Works on macOS, Linux, and Windows (WSL/Git Bash)."
---

# Shell Scripting

Write scripts that fail loudly and safely, not ones that silently do the wrong thing.

## Start every script with a strict header

```bash
#!/usr/bin/env bash
set -euo pipefail   # exit on error, error on unset var, fail a pipeline if any stage fails
IFS=$'\n\t'
```

## Quoting & safety (the top source of bugs)

- Always quote expansions: `"$var"`, `"${arr[@]}"`, `"$(cmd)"` — unquoted values word-split and glob.
- Use `[[ ... ]]` over `[ ... ]` for tests; `(( ... ))` for arithmetic.
- Prefer `"$(cmd)"` over backticks. Check `mkdir -p`, `rm -rf` paths twice.
- Handle filenames with spaces/newlines: `find ... -print0 | xargs -0`, or
```

</details>
