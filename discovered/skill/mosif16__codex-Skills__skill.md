---
name: mosif16__codex-Skills__skill
source: https://github.com/mosif16/codex-Skills/blob/f10bf9466c5287a2766d10d7c1fb2740d5749aee/skills/Rust/Skill.md
repo: mosif16/codex-Skills
kind: skill
stars: 15
last_pushed: 2025-11-25T14:36:56Z
license: unknown
score: 8
domains: [systems-programming, backend]
tags: [rust, best-practices, error-handling, performance]
curated: 2026-06-15
curated_by: config-scout
---

# mosif16/codex-Skills — skill

**Why it's worth keeping:** It prescribes actionable crate usage (thiserror, anyhow) and distinguishes between library and binary patterns. The guidance on error propagation and memory management is directly transferable to an agent's instruction set.

**Summary:** Provides highly specific, opinionated instructions for writing idiomatic and performant Rust code, including project layout and error handling strategies.

**Source credibility:** Moderate; 15 stars indicates a niche but recognized collection of skills.

**Recency:** Current; the instructions reflect modern Rust industry standards and tooling like rustfmt.

**Source:** [mosif16/codex-Skills/skills/Rust/Skill.md](https://github.com/mosif16/codex-Skills/blob/f10bf9466c5287a2766d10d7c1fb2740d5749aee/skills/Rust/Skill.md) · 15★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: "Rust Best Practices Guide"
description: "A comprehensive guide to modern Rust best practices covering style, error handling, performance, concurrency, project organization, dependency management, documentation, testing, security, and CI."
version: "1.0"
dependencies: []
---

# Instructions

## General Coding Conventions and Style

- **Use Standard Naming Conventions:** Follow Rust’s naming idioms for all identifiers. Type names (structs, enums, traits) and enum variants use `UpperCamelCase`. Function, method, module, and variable names use `snake_case`. Constants and statics use `SCREAMING_SNAKE_CASE`. For example, a struct might be named `UserAccount` and a function `process_request`. Avoid acronyms in all-caps in CamelCase (use `Uuid` instead of `UUID`) and prefer full words over abbreviations. If a desired name is a reserved keyword, use a raw identifier (e.g. `r#trait`) or append an underscore rather than misspelling the name.

- **Code Formatting with rustfmt:** Adhere to the official Rust Style Guide (largely embodied by `rustfmt`). Use 4 spaces for indentation and keep line width under 100 chars. Let `rustfmt` automatically format your code to enforce consistent s
```

</details>
