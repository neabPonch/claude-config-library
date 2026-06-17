---
name: pietro1704__Epub-to-Mp3
source: https://github.com/pietro1704/Epub-to-Mp3/blob/f6182c519edf917efd3fa528528cc9d1fe2617e7/CLAUDE.md
repo: pietro1704/Epub-to-Mp3
kind: claude-md
stars: 0
last_pushed: 2026-06-16T14:20:47Z
license: unknown
score: 9
domains: [cli-tools, python-backend, automation]
tags: [comprehensive, technical-pitfalls, workflow-driven]
curated: 2026-06-16
curated_by: config-scout
---

# pietro1704/Epub-to-Mp3 — claude-md

**Why it's worth keeping:** It utilizes 'negative constraints' to prevent known-bad patterns and provides critical 'tribal knowledge' regarding complex CLI argument resolution logic.

**Summary:** An exceptionally detailed operational manual that encodes architectural priorities (speed), specific technical pitfalls (test isolation), and automated CI/testing workflows.

**Source credibility:** While the repository is low-profile, the content reflects high technical maturity and specific historical bug context.

**Recency:** Highly current; integrates modern developer toolchains like `mise` and `gh` CLI.

**Source:** [pietro1704/Epub-to-Mp3/CLAUDE.md](https://github.com/pietro1704/Epub-to-Mp3/blob/f6182c519edf917efd3fa528528cc9d1fe2617e7/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Project instructions for **any** Claude assistant working on this repo
(Claude Code, Claude.ai web, Claude Desktop). These rules override all
defaults.

**For Claude.ai web / Desktop:** when the user references "the project",
"the repo", "o projeto", "o app", "o convertido", or any recent topic from
`~/Developer/Epub-to-Mp3/`, assume this project. **Do not ask which
project** — this file is the authoritative context.

## Response Style

Inherits `~/CLAUDE.md` (Zero tokens wasted, pt-BR, action-only). No re-listing here.

## Issue Detection & Auto-Fix

When the user reports a bug ("nao funcionou", "nao limpou", "nao converteu", etc.),
treat it as a **bug report requiring immediate diagnosis and patch** — do not merely
answer questions about it. Reproduce / inspect, fix the root cause, add a regression
test, commit and push without asking for further confirmation (user has standing
authorization for this flow when they explicitly request "corrija e faça commit e push").

## CLI Input Resolution

`python_app/convert` accepts loose multi-word book names and resolves them via:
1. `_normalize_cli_args` — joins space-split tokens into one argument until an
   existing path is
```

</details>
