---
name: fajarkraton__fajar-lang
source: https://github.com/fajarkraton/fajar-lang/blob/f381b23c485628c8d34534e329307ed81bfc26ef/CLAUDE.md
repo: fajarkraton/fajar-lang
kind: claude-md
stars: 3
last_pushed: 2026-06-12T11:56:52Z
license: apache-2.0
score: 9
domains: [systems-programming, compilers, embedded-ml, cli-tools]
tags: [state-tracking, tdd-workflow, engineering-log, context-grounding]
curated: 2026-06-15
curated_by: config-scout
---

# fajarkraton/fajar-lang — claude-md

**Why it's worth keeping:** It utilizes an advanced 'Mandatory Session Protocol' to enforce TDD and provides a detailed completion status (e.g., [x], [sim], [f]) that prevents AI drift during long-term development cycles.

**Summary:** This file acts as a high-density state machine that tracks granular engineering progress and maintains technical truth through highly specific metrics.

**Source credibility:** High; the document demonstrates extreme technical rigor and detailed version history characteristic of serious systems programming.

**Recency:** Extremely current, utilizing future-dated benchmarks to maintain a high-pressure engineering context.

**Source:** [fajarkraton/fajar-lang/CLAUDE.md](https://github.com/fajarkraton/fajar-lang/blob/f381b23c485628c8d34534e329307ed81bfc26ef/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Fajar Lang Master Reference

> Auto-loaded by Claude Code on every session. This is the **single source of truth** for all development decisions. Read this FIRST before any action.

---

## 1. Project Identity

- **Project:** Fajar Lang (`fj`) — A statically-typed systems programming language for embedded ML + OS integration
- **File extension:** `.fj`
- **Author:** Fajar (TaxPrime / PrimeCore.id)
- **Model:** Claude Opus 4.6 exclusively
- **Stack:** Rust (interpreter/compiler), ndarray (tensor backend), miette (error display), Cranelift (native codegen — v1.0)
- **Binary name:** `fj`

**Vision:** *"Bahasa terbaik untuk embedded ML + OS integration — the only language where an OS kernel and a neural network can share the same codebase, type system, and compiler, with safety guarantees that no existing language provides."*

**Design Principles:**
1. **Explicitness over magic** — no hidden allocation or hidden cost
2. **Dual-context safety** — @kernel disables heap+tensor; @device disables raw pointers. Compiler enforces isolation
3. **Rust-inspired but simpler** — ownership lite without lifetime annotations
4. **Native tensor types** — Tensor is a first-class citizen i
```

</details>
