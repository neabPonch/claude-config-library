---
name: NineWorlds__serenity-android__skill
source: https://github.com/NineWorlds/serenity-android/blob/01adbf2bac2d7431c71e7e0e3ba8a27a8674b7ee/.skills/code-reviewer/SKILL.md
repo: NineWorlds/serenity-android
kind: skill
stars: 201
last_pushed: 2026-05-22T21:41:02Z
license: mit
score: 7
domains: [android, mobile-development]
tags: [code-review, architecture-enforcement, pattern-validation]
curated: 2026-06-15
curated_by: config-scout
---

# NineWorlds/serenity-android — skill

**Why it's worth keeping:** It includes 'Prohibited' lists and explicit cleanup instructions, which are highly effective at preventing AI-generated technical debt and pattern drift.

**Summary:** Acts as a rigorous architectural guardrail that enforces specific patterns for an Android project using Moxy and Toothpick.

**Source credibility:** A specialized open-source media client with moderate community traction.

**Recency:** Current for the project's specific tech stack requirements.

**Source:** [NineWorlds/serenity-android/.skills/code-reviewer/SKILL.md](https://github.com/NineWorlds/serenity-android/blob/01adbf2bac2d7431c71e7e0e3ba8a27a8674b7ee/.skills/code-reviewer/SKILL.md) · 201★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: code-reviewer
description: "Trigger: Pre-Commit/Final Review. Validating code against Serenity’s 'Golden Standards' for architecture, security, performance, and testing before merging."
---

# Code Review Criteria

## Architectural Review
- **MVP Pattern (Moxy)**:
    - Views (`Activity`/`Fragment`) must be "dumb" and passive.
    - Business logic, state, and data fetching must be in the `Presenter`.
- **DI (Toothpick)**:
    - dependencies provided via `Module`.
    - Use `Provider<Presenter>` and `moxyPresenter` delegate (NOT `@InjectPresenter`).
    - Correct scoping (e.g., `APPLICATION_SCOPE`).
    - `@InjectConstructor` usage.
- **Repository Pattern**: Presenters must use Repositories, not API clients directly.

## Security & Reliability
- **Data Handling**: No sensitive data in logs/hardcoded. Input validation.
- **Networking**: HTTPS via Retrofit.
- **Error Handling**: Use `executeOrThrow()` for consistent propagation.
- **Prohibited**: No Retrofit `.enqueue()`. Use Coroutines.

## Performance
- **Concurrency**: Heavy ops on `Dispatchers.IO`/`Default`. Correct `CoroutineScope` management.
- **Resource Management**: No Context leaks. Proper unregistration of listene
```

</details>
