---
name: databricks-solutions__apx__skill
source: https://github.com/databricks-solutions/apx/blob/a88ee32f22669eac0df57198006bdba7db44a878/.claude/skills/rust/SKILL.md
repo: databricks-solutions/apx
kind: skill
stars: 82
last_pushed: 2026-04-07T17:22:25Z
license: other
score: 9
domains: [systems-programming, backend]
tags: [rust, coding-standards, safety-critical, ddd]
curated: 2026-06-15
curated_by: config-scout
---

# databricks-solutions/apx — skill

**Why it's worth keeping:** It provides highly specific technical constraints (e.g., '#[expect]' vs '#[allow]') and actionable 'bad vs good' examples that prevent mediocre LLM output.

**Summary:** A rigorous, expert-level Rust development standard covering safety, naming, error handling, and architectural patterns.

**Source credibility:** High; derived from a Databricks-associated engineering toolkit.

**Recency:** Very current, utilizing modern Rust linting and architectural standards.

**Source:** [databricks-solutions/apx/.claude/skills/rust/SKILL.md](https://github.com/databricks-solutions/apx/blob/a88ee32f22669eac0df57198006bdba7db44a878/.claude/skills/rust/SKILL.md) · 82★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: rust
description: Strict set of rules in terms of codebase development, design patterns, and best practices. Use when the user wants to develop a new feature or refactor existing code.
---

## Principles

Priority: **Correctness > Safety > Readability > Performance**

- **Idiomatic Rust.** Follow standard library conventions. If the stdlib does it one way, do it that way.
- **Leverage the type system.** Encode invariants in types, not runtime checks. Make illegal states unrepresentable.
- **Domain-driven design.** Name everything in the language of the problem, not the implementation.
- **Reuse existing libraries and frameworks** when possible.

## Safety rules

Adapted from [The Power of Ten](https://en.wikipedia.org/wiki/The_Power_of_10:_Rules_for_Developing_Safety-Critical_Code) (Holzmann) for Rust.

1. **Simple control flow.** No nested if-else, no nested loops. Split into single-purpose functions. Max one level of branching per function body.
2. **Short functions.** No function longer than ~60 lines. If it's too long, decompose it.
3. **Fixed loop bounds.** All loops must have a provable upper bound. Prefer iterators (`for x in collection`) over manual `while i < len
```

</details>
