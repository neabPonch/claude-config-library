---
name: bushidocodes__limerick-cobol
source: https://github.com/bushidocodes/limerick-cobol/blob/e92ada13b43fd1375a1e0b05625f7660275e9a96/CLAUDE.md
repo: bushidocodes/limerick-cobol
kind: claude-md
stars: 2
last_pushed: 2026-06-14T20:13:24Z
license: unknown
score: 9
domains: [web-frontend, static-site, devops]
tags: [build-process, git-workflow, visual-debugging, generated-files]
curated: 2026-06-15
curated_by: config-scout
---

# bushidocodes/limerick-cobol — claude-md

**Why it's worth keeping:** The 'Generated files' mapping table prevents the agent from editing build output, and the visual bug investigation protocol optimizes debugging by prioritizing tool-based screenshots over code analysis.

**Summary:** A highly rigorous guide for a static site project that manages complex build-step mappings and strict Git workflows.

**Source credibility:** Low star count (2) but demonstrates extremely high technical discipline in documentation.

**Recency:** Very current; utilizes specific Claude Code capabilities like preview_start and preview_inspect.

**Source:** [bushidocodes/limerick-cobol/CLAUDE.md](https://github.com/bushidocodes/limerick-cobol/blob/e92ada13b43fd1375a1e0b05625f7660275e9a96/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Limerick COBOL

Static site for COBOL programming exercises. Exercise, lecture, and course pages are hand-authored HTML; example pages (`examples/**/*.html`) are **generated** — see [Generated files](#generated-files) before editing anything under `examples/`.

## Before starting any work

Fetch, then check that the branch is current with master:

```bash
git fetch origin
git rev-list --count HEAD..origin/master
```

**Always run `git fetch origin` first.** Without it, the local remote-tracking ref may be stale and the count will appear to be 0 even when origin/master has moved ahead.

If the count is greater than 0, rebase **before** making any changes:

```bash
git rebase origin/master
```

If the current branch has already been merged into master, create a fresh branch from origin/master instead of adding more commits to it:

```bash
git checkout -b fix/<description> origin/master
```

A stale branch inflates the PR diff with unrelated commits and causes conflicts on stash pop. Never use `git stash + git rebase + git stash pop` — commit work-in-progress first, then rebase.

## Validation

```bash
npm run validate
```

Runs `html-validate` against all HTML pages. Run after any
```

</details>
