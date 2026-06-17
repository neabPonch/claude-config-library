---
name: matthewharwood__engmanager.xyz__010-crud-pattern-skill
source: https://github.com/matthewharwood/engmanager.xyz/blob/09c826330280721807a7be19f8a9b5a9b6c210de/prompts/010-crud-pattern-skill.md
repo: matthewharwood/engmanager.xyz
kind: skill
stars: 3
last_pushed: 2026-06-13T22:21:05Z
license: unknown
score: 9
domains: [backend-api, rust, architecture]
tags: [axum, crud, repository-pattern, rust]
curated: 2026-06-15
curated_by: config-scout
---

# matthewharwood/engmanager.xyz — skill

**Why it's worth keeping:** It enforces a professional layered architecture (Repository/Service/Handler) and provides clear strategies for trait-based database portability.

**Summary:** A rigorous architectural blueprint for generating production-grade CRUD pattern skills in Rust using the Axum framework.

**Source credibility:** High; authored by an engineering leader focused on systems and scale.

**Recency:** Current; aligns with modern Axum, Tokio, and async-trait patterns.

**Source:** [matthewharwood/engmanager.xyz/prompts/010-crud-pattern-skill.md](https://github.com/matthewharwood/engmanager.xyz/blob/09c826330280721807a7be19f8a9b5a9b6c210de/prompts/010-crud-pattern-skill.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Create CRUD Pattern Skill Document

<objective>
Create a production-quality skill document for implementing reusable CRUD patterns in Axum applications, based on the research conducted in the previous step.

This skill will enable developers to rapidly add CRUD operations for any entity while maintaining type safety, testability, and database portability.
</objective>

<context>
## Research Foundation

Read the comprehensive research document:
@./research/crud-pattern-analysis.md

This research provides:
- Trait designs
- Architecture patterns
- Implementation strategies
- Code examples
- Best practices

Your task is to transform this research into a clear, actionable skill document.

## Target Audience

Developers who need to:
- Add CRUD operations for new entities (routes, users, posts, etc.)
- Migrate from JSON files to databases
- Maintain type safety and testability
- Follow Axum service architecture patterns

## Related Skills

The CRUD skill should integrate with:
- axum-service-architecture (layered design, AppState, FromRef)
- axum-web-framework (handlers, extractors, error handling)
- rust-core-patterns (newtypes, traits, type states)
- rust-error-handling (error types,
```

</details>
