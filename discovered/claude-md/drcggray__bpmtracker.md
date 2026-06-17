---
name: drcggray__bpmtracker
source: https://github.com/drcggray/bpmtracker/blob/2d2acf63b63087534325a8524d638fe091df97da/claude.md
repo: drcggray/bpmtracker
kind: claude-md
stars: 0
last_pushed: 2025-06-18T22:28:07Z
license: unknown
score: 8
domains: [general-dev, tdd, frontend]
tags: [discipline, tdd, documentation, ux]
curated: 2026-06-15
curated_by: config-scout
---

# drcggray/bpmtracker — claude-md

**Why it's worth keeping:** The 'ABOUTME:' greppable comment pattern, the rigid 6-step TDD loop, and the mandate for 'smallest reasonable changes' are highly transferable guardrails.

**Summary:** This config enforces extreme discipline through strict TDD mandates, file-size constraints, and specific documentation standards. It is designed to prevent AI-driven code rot and technical debt.

**Source credibility:** Low social proof (0 stars), but demonstrates high-level developer discipline.

**Recency:** Repository is a year old, but these behavioral constraints remain highly relevant for modern agentic coding.

**Source:** [drcggray/bpmtracker/claude.md](https://github.com/drcggray/bpmtracker/blob/2d2acf63b63087534325a8524d638fe091df97da/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Working with Jesse

## Code Writing

- YOU MUST ALWAYS address me as "George" in all communications.
- We STRONGLY prefer simple, clean, maintainable solutions over clever or complex ones. Readability and maintainability are PRIMARY CONCERNS, even at the cost of conciseness or performance.
- YOU MUST make the SMALLEST reasonable changes to achieve the desired outcome.
- Aim to keep files sizes to no more than 300-400 lines, and if you need more lines in a file think about refactoring.
- YOU MUST MATCH the style and formatting of surrounding code, even if it differs from standard style guides. Consistency within a file trumps external standards.
- YOU MUST NEVER make code changes unrelated to your current task. If you notice something that should be fixed but is unrelated, document it rather than fixing it immediately.
- YOU MUST NEVER remove code comments unless you can PROVE they are actively false. Comments are important documentation and must be preserved.
- All code files MUST start with a brief 2-line comment explaining what the file does. Each line MUST start with "ABOUTME: " to make them easily greppable.
- YOU MUST NEVER refer to temporal context in comments (like "recent
```

</details>
