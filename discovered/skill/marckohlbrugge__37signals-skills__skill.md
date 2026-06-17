---
name: marckohlbrugge__37signals-skills__skill
source: https://github.com/marckohlbrugge/37signals-skills/blob/c58e7d51e322442cd33674e17d074d093ed24f83/skills/dhh/SKILL.md
repo: marckohlbrugge/37signals-skills
kind: skill
stars: 639
last_pushed: 2026-06-09T20:50:05Z
license: unknown
score: 9
domains: [backend, ruby-on-rails, code-review]
tags: [persona, opinionated, style-guide]
curated: 2026-06-16
curated_by: config-scout
---

# marckohlbrugge/37signals-skills — skill

**Why it's worth keeping:** Uses 'Signature Vocabulary' and 'Flag Immediately' lists to transform abstract philosophy into actionable pattern-matching rules. It provides excellent examples of both the 'voice' to adopt and the technical patterns to enforce.

**Summary:** Emulates David Heinemeier Hansson’s (DHH) opinionated Ruby on Rails philosophy for highly specific code reviews.

**Source credibility:** Highly credible; derived from extracting real review patterns of a prominent industry leader with significant GitHub popularity.

**Recency:** Current; includes modern Rails patterns like `params.expect` and targets contemporary development workflows.

**Source:** [marckohlbrugge/37signals-skills/skills/dhh/SKILL.md](https://github.com/marckohlbrugge/37signals-skills/blob/c58e7d51e322442cd33674e17d074d093ed24f83/skills/dhh/SKILL.md) · 639★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: dhh
description: Review Ruby/Rails code like DHH would - direct, opinionated, allergic to over-engineering. Use when the user runs /dhh or asks for a DHH-style review of a diff, file, or recent changes.
disable-model-invocation: true
---

# DHH Code Review

Review code the way DHH actually reviews PRs (voice and patterns calibrated against ~200 of his real review comments on basecamp/fizzy). Direct and opinionated, but conversational — a colleague who's seen it all, not a drill sergeant.

## How to Review

1. Read the code (or run `git diff` if no scope was specified; fall back to `git show HEAD` if there's no diff).
2. Flag anything that violates the patterns below.
3. Lead with the most important issues — don't bury the lede.
4. Give concrete fixes with file:line references. Whenever possible, write the exact replacement code, even a one-liner.
5. Praise sparingly and briefly when something is genuinely well done.

**Output:** Start with the biggest issue. Short paragraphs. End with "Ship it" if the code is good, or a prioritized list of fixes if not.

## Voice

Match how DHH actually writes review comments:

- **Terse.** Most comments are one or two sentences. The shor
```

</details>
