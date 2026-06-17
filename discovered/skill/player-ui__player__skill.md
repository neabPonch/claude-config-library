---
name: player-ui__player__skill
source: https://github.com/player-ui/player/blob/3ef62af2592c24b62ba425897125591ab1eb6121/.claude/skills/ios-review/SKILL.md
repo: player-ui/player
kind: skill
stars: 83
last_pushed: 2026-06-16T03:22:34Z
license: mit
score: 9
domains: [ios, swift, swiftui]
tags: [code-review, ios, swift]
curated: 2026-06-16
curated_by: config-scout
---

# player-ui/player — skill

**Why it's worth keeping:** Uses the 'Rule/Why/Example' pattern to ground the AI's reasoning; includes high-value domain expertise like SwiftUI structural identity rules that standard linters often miss.

**Summary:** A rigorous iOS code review persona that enforces strict Swift and SwiftUI standards regarding memory management, concurrency, and view identity.

**Source credibility:** High; originates from a specialized UI framework repository with recent maintenance activity.

**Recency:** Current; incorporates modern Swift concurrency patterns like async/await and Task closures.

**Source:** [player-ui/player/.claude/skills/ios-review/SKILL.md](https://github.com/player-ui/player/blob/3ef62af2592c24b62ba425897125591ab1eb6121/.claude/skills/ios-review/SKILL.md) · 83★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ios-review
description: Review Swift/iOS code against team conventions. Use when the user asks to review Swift code, runs /ios-review, or when writing or editing Swift files in this repo. Enforces standards that linters cannot catch.
context: fork
---

## Current diff (when reviewing a PR)
Get the diff between this branch and its parent branch (NOT always main). If this has no parent branch, stop.

# iOS Code Review — Team Conventions

Review the code (or the diff above if present) against the rules below. Apply **General Rules** always. Apply **UI Rules** only if the changes include SwiftUI views (files containing `View`, `body`, `@ViewBuilder`, or SwiftUI imports).

For each violation, report:
- **Rule**: which rule was broken
- **Location**: file + line number
- **Suggestion**: concrete fix

If no violations are found, say so clearly.

---

## Authoritative Style Guides

Apply these guides in full during every review:

1. **[Swift API Design Guidelines](https://www.swift.org/documentation/api-design-guidelines/)** — naming, documentation, Boolean assertions, protocol suffixes, factory method prefixes, mutating/nonmutating pairs, parameter ordering.
2. **[Google Swift S
```

</details>
