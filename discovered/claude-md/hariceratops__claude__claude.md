---
name: hariceratops__claude__claude
source: https://github.com/hariceratops/claude/blob/73e8676270da04dde4376d143460c0ffbc500c3f/.claude/CLAUDE.md
repo: hariceratops/claude
kind: claude-md
stars: 0
last_pushed: 2026-05-15T08:21:17Z
license: apache-2.0
score: 8
domains: [embedded-systems, systems-programming, rust, cpp]
tags: [low-level, strict-constraints, embedded]
curated: 2026-06-16
curated_by: config-scout
---

# hariceratops/claude — claude-md

**Why it's worth keeping:** It utilizes highly specific negative constraints (what NOT to do) and provides clear, actionable error-handling patterns that prevent common low-level pitfalls.

**Summary:** Establishes rigorous coding standards for low-level systems programming and embedded environments across C, C++, Rust, and Python.

**Source credibility:** Personal configuration repository with minimal social proof.

**Recency:** Current; reflects modern systems programming practices compatible with current AI coding workflows.

**Source:** [hariceratops/claude/.claude/CLAUDE.md](https://github.com/hariceratops/claude/blob/73e8676270da04dde4376d143460c0ffbc500c3f/.claude/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Global Rules

## About Me
SW engineer; primary languages C, C++, Rust, Python.
Projects range from hosted CLI tools and prototypes to bare-metal embedded firmware.

## Code Constraints
- No unnecessary abstractions — solve the problem at hand
- No comments explaining WHAT code does; only WHY (non-obvious rationale)
- No half-finished implementations — stop and say so if incomplete
- No error handling for impossible cases; no unnecessary defensive code

## Language Rules

### Python
- Prefer Result-like error objects over raising exceptions
- Avoid bare `except`; be explicit about caught types when exceptions used
- Type-annotate all function signatures

### Rust
- Idiomatic Result/Option throughout — never unwrap()/expect() in production paths
- Use `thiserror` for library errors, `anyhow` for binary/tool errors

### C / C++
- Explicit error returns (errno-style int codes or typed enums)
- Headers declare interfaces only; implementations in .c/.cpp

## Embedded Systems
Rules that apply only when the project targets bare-metal or RTOS environments
(presence of linker scripts, cross-compilation targets, or no-std Cargo config):

- Minimal dynamic allocation — prefer stack or
```

</details>
