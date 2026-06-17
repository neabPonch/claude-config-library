---
name: InsertKoinIO__koin__claude
source: https://github.com/InsertKoinIO/koin/blob/fff5291f333c04fe5d6d9447f72740647d40d186/projects/CLAUDE.md
repo: InsertKoinIO/koin
kind: claude-md
stars: 9986
last_pushed: 2026-06-15T07:24:41Z
license: apache-2.0
score: 10
domains: [kotlin, kmp, android]
tags: [dependency-injection, multiplatform, testing-rigor]
curated: 2026-06-15
curated_by: config-scout
---

# InsertKoinIO/koin — claude-md

**Why it's worth keeping:** Includes high-signal technical gotchas (like the backtick naming constraint) and a meta-instructionary 'Surprise Rule' to handle documentation gaps. The instruction to 'falsify, don't confirm' provides a superior mental model for AI test generation.

**Summary:** A masterclass in context-setting that includes architectural dogmas, platform-specific 'traps,' and specific testing requirements for Kotlin Multiplatform.

**Source credibility:** High; Koin is a major industry-standard dependency injection framework for Kotlin.

**Recency:** Extremely current, addressing modern technical constraints like WasmJS and Kotlin/Native specificities.

**Source:** [InsertKoinIO/koin/projects/CLAUDE.md](https://github.com/InsertKoinIO/koin/blob/fff5291f333c04fe5d6d9447f72740647d40d186/projects/CLAUDE.md) · 9986★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Koin

Koin is a pragmatic, lightweight dependency injection framework for Kotlin Multiplatform (Android, JVM, iOS/native, JS, WasmJS). This directory (`projects/`) is the Gradle build root.

## Doctrine

- **Evidence-based claims.** "fixed/verified/done" must cite file:line, test output, or a repro run — never "looks right + tests pass".
- **Falsify, don't confirm.** A test must try to BREAK the implementation. Prove RED before GREEN: a regression test must fail on the unfixed code.
- **Resolution behavior is a contract.** Koin's resolution order/matching semantics are user-observable API — treat any change there as a compatibility event, not an implementation detail.

> **SURPRISE RULE — mandatory.** If the project surprises you or contradicts these docs, STOP, tell the user, and record it here (or in the closest module doc). "Surprising" = not inferable from the code in one grep.

## Module Map

| Group | Modules | Notes |
|---|---|---|
| `core/` | **koin-core** (engine), koin-core-coroutines, koin-core-viewmodel, koin-core-annotations, koin-annotations, koin-test, koin-test-junit4/5, benchmark | KMP |
| `android/` | koin-android, koin-android-compat, koin-androidx-navigation,
```

</details>
