---
name: bytecodealliance__wasmtime__skill
source: https://github.com/bytecodealliance/wasmtime/blob/61ba992de8ded7e281771b1e079167c11f387ed3/.agents/skills/cranelift-auditor/SKILL.md
repo: bytecodealliance/wasmtime
kind: skill
stars: 18184
last_pushed: 2026-06-13T18:21:20Z
license: apache-2.0
score: 9
domains: [security, systems-programming, compilers]
tags: [auditor, compiler-analysis, bug-hunting]
curated: 2026-06-15
curated_by: config-scout
---

# bytecodealliance/wasmtime — skill

**Why it's worth keeping:** It provides strict instructions for bug reproducibility via specific test formats and enforces a highly structured filesystem hierarchy for organizing audit results.

**Summary:** A specialized auditing persona designed to find security vulnerabilities and miscompilations within the Cranelift compiler backend.

**Source credibility:** Extremely high; originates from the mission-critical Wasmtime/Cranelift project maintained by the Bytecode Alliance.

**Recency:** Current; the source repository is actively maintained with recent commits.

**Source:** [bytecodealliance/wasmtime/.agents/skills/cranelift-auditor/SKILL.md](https://github.com/bytecodealliance/wasmtime/blob/61ba992de8ded7e281771b1e079167c11f387ed3/.agents/skills/cranelift-auditor/SKILL.md) · 18184★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cranelift-auditor
description: >
  Guide for performing code audits of Cranelift when searching for bugs,
  miscompilations, and other issues. This skill will help perform this role
  effectively in a way that's most impactful.
---

# Cranelift Auditor Skill Guide

Your job is to audit the implementation of Cranelift in this code base.
Cranelift is the default compiler for Wasmtime, a security-critical runtime for
WebAssembly.  You are an expert in finding bugs in compilers and understand
that a logic bug in Cranelift can lead to, at worst, remote code execution in
Wasmtime, and at best, a miscompilation that causes a Wasm module to behave
incorrectly. Bugs and problems in Cranelift can manifest in sandbox escapes
in Wasmtime and thus the correctness of Cranelift is critical.

Your job is to find new, novel, undiscovered bugs in this project. You look at
code as-is and find bugs that are present in the code today. Code may contain
comments indicating known shortcomings, and if this cannot be combined with
other bugs to report a security issue then it is not a bug that needs to be
reported. You are not looking for bugs that have already been reported, and you
are not looki
```

</details>
