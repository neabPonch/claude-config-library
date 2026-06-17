---
name: sanogueralorenzo__sanogueralorenzo.github.io__skill
source: https://github.com/sanogueralorenzo/sanogueralorenzo.github.io/blob/936db58bffd713956a2d2854a6e5f2a7c3ce25ae/skills/pr-review/SKILL.md
repo: sanogueralorenzo/sanogueralorenzo.github.io
kind: skill
stars: 1786
last_pushed: 2026-06-11T06:52:45Z
license: mit
score: 8
domains: [software-engineering, devops, cli-tools]
tags: [code-review, workflow, multi-pass]
curated: 2026-06-14
curated_by: config-scout
---

# sanogueralorenzo/sanogueralorenzo.github.io — skill

**Why it's worth keeping:** The multi-turn architecture prevents detail loss; it provides specific heuristics like 'domain names over implementation details' which are highly transferable.

**Summary:** A sophisticated multi-pass workflow that breaks down PR reviews into specialized stages for logic, simplification, naming, and documentation.

**Source credibility:** High star count suggests a well-regarded collection of personal configurations/dotfiles.

**Recency:** Extremely current, with activity in the current month.

**Source:** [sanogueralorenzo/sanogueralorenzo.github.io/skills/pr-review/SKILL.md](https://github.com/sanogueralorenzo/sanogueralorenzo.github.io/blob/936db58bffd713956a2d2854a6e5f2a7c3ce25ae/skills/pr-review/SKILL.md) · 1786★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pr-review
description: Multi-turn pull request review workflow. Use when reviewing a GitHub PR with local Codex tooling, gh, and acli; runs a general review first, then focused simplification, naming, and documentation passes.
---

# PR Review

Review pull requests in four focused turns. Assume `gh`, `acli`, `codex`, and `codex-core` are installed and authenticated before starting. Do not install tools or change repository code during review.

## Operating Rules

- State assumptions before running the review.
- Ask only when the PR target, publish mode, or repository context is ambiguous.
- Review the diff and surrounding code, not only the patch.
- Prefer concrete bugs, regressions, missing tests, and confusing code over style opinions.
- Keep findings concise and actionable.
- Do not invent risk. If a concern is speculative, label it as speculative or omit it.
- Post findings after each pass when the workflow is configured to publish incrementally.

## Workflow

1. General review
   - Check correctness, regressions, data flow, async behavior, error states, security-sensitive paths, and test gaps.
   - Prioritize issues that could break user-visible behavior or productio
```

</details>
