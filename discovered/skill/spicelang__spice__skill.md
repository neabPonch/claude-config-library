---
name: spicelang__spice__skill
source: https://github.com/spicelang/spice/blob/35379f9a7b843547552e9227ab35fbc83a6f5fd6/.claude/skills/spice-contribute/SKILL.md
repo: spicelang/spice
kind: skill
stars: 86
last_pushed: 2026-06-14T22:54:35Z
license: mit
score: 9
domains: [systems-programming, compilers]
tags: [workflow, verification, git]
curated: 2026-06-15
curated_by: config-scout
---

# spicelang/spice — skill

**Why it's worth keeping:** It provides concrete CLI commands for build/test validation, transforming vague quality gates into actionable instructions an agent can execute to prove its work.

**Summary:** Defines rigorous contribution workflows including branch naming conventions, commit protocols, and explicit verification steps for the Spice compiler.

**Source credibility:** High; part of a live language development repository.

**Recency:** 

**Source:** [spicelang/spice/.claude/skills/spice-contribute/SKILL.md](https://github.com/spicelang/spice/blob/35379f9a7b843547552e9227ab35fbc83a6f5fd6/.claude/skills/spice-contribute/SKILL.md) · 86★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: spice-contribute
description: Guidelines for contributing changes to the Spice GitHub repository — branch naming conventions, commit message format, PR workflow, no-push-to-main rule, and quality gates. Use when preparing a branch for review, writing a commit, opening a PR, or checking that a contribution is ready to merge.
---

# Contribute to Spice

This skill covers the full contribution workflow: naming branches, writing
commits, opening a PR, and satisfying the quality gates before merge.

## Branch naming

All work happens on a dedicated branch, never directly on `main`.

| Prefix | Use for |
|--------|---------|
| `feature/<slug>` | New language features, compiler capabilities, or stdlib additions |
| `fix/<slug>` | Bug fixes in the compiler, runtime, or stdlib |
| `chore/<slug>` | Build system, dependency updates, repo maintenance |
| `ci/<slug>` | GitHub Actions workflows, CI scripts, test infrastructure |
| `std/<slug>` | Standard library changes that aren't strictly a new feature or fix |
| `bootstrap/<slug>` | Changes to the self-hosted bootstrap compiler (`src-bootstrap/`) |
| `test/<slug>` | New or updated test cases, test utilities, reference files |
| `doc
```

</details>
