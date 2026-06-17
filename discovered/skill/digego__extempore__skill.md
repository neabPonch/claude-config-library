---
name: digego__extempore__skill
source: https://github.com/digego/extempore/blob/8ff862c87ba9a2157cc6b6ba17c7dee009bd94f5/.claude/skills/extempore-debugging/SKILL.md
repo: digego/extempore
kind: skill
stars: 1461
last_pushed: 2026-06-10T11:36:28Z
license: unknown
score: 9
domains: [systems-programming, compiler-engineering, debugging]
tags: [architecture, jit, llvmir, troubleshooting]
curated: 2026-06-15
curated_by: config-scout
---

# digego/extempore — skill

**Why it's worth keeping:** It maps out exact process flows for JIT/AOT compilation and provides highly specific 'gotcha' examples (like the xtlang `set!` type error) that are crucial for debugging.

**Summary:** Provides deep architectural insights into the Extempore runtime, including compilation paths and how different execution modes affect global state.

**Source credibility:** High; based on a well-regarded repository with significant community interest (1461 stars).

**Recency:** Current; reflects modern low-level system/JIT complexities.

**Source:** [digego/extempore/.claude/skills/extempore-debugging/SKILL.md](https://github.com/digego/extempore/blob/8ff862c87ba9a2157cc6b6ba17c7dee009bd94f5/.claude/skills/extempore-debugging/SKILL.md) · 1461★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: extempore-debugging
description: Debugging and development guide for Extempore. Use when debugging JIT compilation issues, understanding symbol tracking, or testing compilation in different modes (batch, eval, interactive).
---

# Extempore debugging skill

## Architecture overview

Extempore has three main layers:

1. **C++ runtime** (`src/`): Scheme interpreter, LLVM JIT, audio/OSC
2. **Scheme runtime** (`runtime/`): scheme.xtm, llvmir.xtm, llvmti.xtm
3. **xtlang libraries** (`libs/`): user-facing compiled DSL code

## Compilation paths

### Normal (interactive) compilation

```
llvm:compile-ir
  -> llvm:jit-compile-ir-string (Scheme FFI)
    -> jitCompile() in src/SchemeFFI.cpp
      -> initializeTemplateModule() parses runtime/bitcode.ll once
      -> parseAssemblyInto() of (type defs + user IR)
      -> EXTLLVM::addTrackedModule() (ORC JIT)
      -> EXTLLVM::addModule() (metadata tracking)
```

### AOT compilation

When `*impc:aot:current-output-port*` is set:

```
llvm:compile-ir
  -> impc:compiler:queue-ir-for-compilation
    -> appends to *impc:compiler:queued-llvm-ir-string*

impc:compiler:flush-jit-compilation-queue
  -> llvm:jit-compile-ir-string with accumulat
```

</details>
