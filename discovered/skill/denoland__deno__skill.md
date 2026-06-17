---
name: denoland__deno__skill
source: https://github.com/denoland/deno/blob/3346df152c7b9c6a166f7e15c8149af355ab8d74/.claude/skills/review-pr/SKILL.md
repo: denoland/deno
kind: skill
stars: 107085
last_pushed: 2026-06-15T08:09:12Z
license: mit
score: 9
domains: [cli-tools, security, backend-runtime, open-source]
tags: [code-review, ci-cd, rust, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# denoland/deno — skill

**Why it's worth keeping:** It follows an elite agentic pattern: first gathering context via CLI, then applying strict 'gate' criteria (CI, title format) before diving into deep technical heuristics for Rust and JS/TS.

**Summary:** A highly specialized skill that transforms Claude into a senior Deno maintainer by implementing multi-stage gatekeeping and domain-specific technical checks.

**Source credibility:** Extremely high; derived from the official Deno repository context used by its core contributors.

**Recency:** Current; utilizes modern GitHub CLI patterns and sophisticated tool-calling logic compatible with Claude Code.

**Source:** [denoland/deno/.claude/skills/review-pr/SKILL.md](https://github.com/denoland/deno/blob/3346df152c7b9c6a166f7e15c8149af355ab8d74/.claude/skills/review-pr/SKILL.md) · 107085★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: review-pr
description: Review a Deno runtime pull request for correctness, tests, security, and conventions. Use when asked to review a PR or when a PR number/URL is provided for review.
argument-hint: <pr-number-or-url>
allowed-tools: Bash(gh *) Bash(git *) Read Glob Grep Agent
---

# Deno PR Reviewer

Review PR `$ARGUMENTS` on the `denoland/deno` repository.

## Step 1: Gather PR context

Fetch the PR metadata, diff, and comments:

```!
gh pr view $ARGUMENTS --json number,title,body,author,labels,state,reviewDecision,commits,files,isDraft,createdAt,url
```

```!
gh pr diff $ARGUMENTS
```

```!
gh pr view $ARGUMENTS --comments --json comments
```

```!
gh pr checks $ARGUMENTS --json name,state,conclusion 2>/dev/null || echo "No checks found"
```

## Step 2: Gate checks

Before reviewing code, check these gates. If any fail, flag them prominently at
the top of your review and do not approve.

1. **CI status** — All checks must pass. Point the author to specific failing
   checks. Known flaky tests (labeled `ci-test-flaky`) can be re-run.
2. **PR title format** — Must follow `type(scope): description`. Types: `feat`,
   `fix`, `perf`, `refactor`, `chore`, `docs`, `test`, `
```

</details>
