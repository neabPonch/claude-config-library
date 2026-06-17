---
name: backengineering__llvm-msvc__skill
source: https://github.com/backengineering/llvm-msvc/blob/969674f34d70361541cac07f28154af5f4469eba/.agents/skills/dynamic-instrumentation/SKILL.md
repo: backengineering/llvm-msvc
kind: skill
stars: 422
last_pushed: 2026-06-05T13:16:54Z
license: agpl-3.0
score: 9
domains: [systems-programming, security, compiler-engineering]
tags: [llvm, dbi, instrumentation, profiling, qbdi]
curated: 2026-06-15
curated_by: config-scout
---

# backengineering/llvm-msvc — skill

**Why it's worth keeping:** Provides concrete implementation patterns for LLVM IR passes, SanitizerCoverage callbacks, and QBDI runtime interception that are highly specific and non-trivial.

**Summary:** A high-density technical guide for dynamic binary instrumentation and compile-time code transformation using LLVM infrastructure.

**Source credibility:** High; based on a specialized LLVM fork with active maintenance and significant community interest.

**Recency:** 

**Source:** [backengineering/llvm-msvc/.agents/skills/dynamic-instrumentation/SKILL.md](https://github.com/backengineering/llvm-msvc/blob/969674f34d70361541cac07f28154af5f4469eba/.agents/skills/dynamic-instrumentation/SKILL.md) · 422★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: dynamic-instrumentation
description: Expertise in LLVM-based dynamic binary instrumentation, runtime tracing, and program monitoring. Use this skill when implementing runtime analysis tools, code coverage systems, profilers, or dynamic security monitors.
---

# Dynamic Instrumentation Skill

This skill covers dynamic binary instrumentation (DBI), runtime tracing, and program monitoring using LLVM infrastructure.

## Dynamic Binary Instrumentation Overview

### What is DBI?
Dynamic Binary Instrumentation allows modifying program behavior at runtime without source code access:
- Insert analysis code at arbitrary points
- Monitor program execution
- Modify control flow and data

### LLVM-Based DBI Tools
- **QBDI**: QuarkslaB Dynamic Binary Instrumentation
- **Instrew**: Fast instrumentation through LLVM lifting
- **binopt**: Runtime optimization of binary code

## QBDI (QuarkslaB DBI)

### Basic Usage
```cpp
#include <QBDI.h>

// Callback function for instrumentation
QBDI::VMAction onInstruction(QBDI::VMInstanceRef vm, 
                              QBDI::GPRState *gprState,
                              QBDI::FPRState *fprState, 
                              void *data) {
```

</details>
