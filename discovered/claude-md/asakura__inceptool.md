---
name: asakura__inceptool
source: https://github.com/asakura/inceptool/blob/9e52f9954ff06cd01ea6cc0313626638cb4ca1a3/CLAUDE.md
repo: asakura/inceptool
kind: claude-md
stars: 0
last_pushed: 2026-06-15T08:04:37Z
license: apache-2.0
score: 9
domains: [rust, systems-programming, cli-tools]
tags: [rust, error-handling, testing-patterns, high-performance]
curated: 2026-06-15
curated_by: config-scout
---

# asakura/inceptool — claude-md

**Why it's worth keeping:** It prevents 'lazy' coding by banning .unwrap() even in tests and mandates specific error-wrapping strategies that ensure type safety.

**Summary:** Enforces strict Rust error handling, testing hygiene, and zero-copy design patterns across a workspace.

**Source credibility:** Individual developer project with very recent activity.

**Recency:** 

**Source:** [asakura/inceptool/CLAUDE.md](https://github.com/asakura/inceptool/blob/9e52f9954ff06cd01ea6cc0313626638cb4ca1a3/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## RULES

- errors: `thiserror` enums in lib crates (protocol/engine/drivers/hooks);
  `miette` for cli terminal output. All errors MUST be wrapped by the crate's
  `Error` type (e.g. `ProtocolError` in error.rs).
- testing: no `.unwrap()`/`.expect()` anywhere, incl. tests; use `?` -> crate's
  `Result` (or `miette::Result` in integration tests); prefer
  `core::assert_matches!` over manual matches.
- test-errors: each `mod tests` defines its own private `TestError` (`thiserror`),
  not a shared/global one; don't reuse domain errors (e.g. `ProtocolError`) for
  test logic; include `Failure(String)` for test-specific panics (note:
  thiserror can't `#[from] String`, since `String` has no `std::error::Error`
  impl).
- test-structure: colocate tests w/ units; keep hyper-specific - split broad
  tests via `rstest` + fixtures/cases/matricies.
- naming: inner crates prefixed `inceptool-` (e.g. `inceptool-protocol`); folder
  paths unchanged.
- design: zero-copy by default; use `Cow<'a, str>` and
  `serde_json::value::RawValue` (`RawJson`) extensively.
- arch: middleware follows Elixir Phoenix `Plug`, but with `&mut Conn` (mutable,
  not immutable) for perf/simplicity in Rus
```

</details>
