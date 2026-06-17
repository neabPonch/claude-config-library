---
name: gmh5225__awesome-llvm-security__skill
source: https://github.com/gmh5225/awesome-llvm-security/blob/32a9d49ee7d8ed3044e23fa3191338430e198315/.claude/skills/dynamic-instrumentation/SKILL.md
repo: gmh5225/awesome-llvm-security
kind: skill
stars: 841
last_pushed: 2026-06-07T15:56:29Z
license: mit
score: 9
domains: [security, systems-programming, compiler-engineering]
tags: [llvm, dbi, instrumentation, profiling]
curated: 2026-06-15
curated_by: config-scout
---

# gmh5225/awesome-llvm-security — skill

**Why it's worth keeping:** The specific C++ boilerplates for `llvm::PassInfoMixin` and Sanitizer Coverage callbacks are highly transferable for writing low-level analysis tools.

**Summary:** Provides high-density technical implementation patterns for LLVM IR passes, dynamic binary instrumentation via QBDI, and compiler-level coverage techniques.

**Source credibility:** Highly credible; sourced from a well-regarded 'awesome' security repository with significant stars and active maintenance.

**Recency:** Current; uses modern LLVM pass patterns and up-to-date instrumentation frameworks like XRay and QBDI.

**Source:** [gmh5225/awesome-llvm-security/.claude/skills/dynamic-instrumentation/SKILL.md](https://github.com/gmh5225/awesome-llvm-security/blob/32a9d49ee7d8ed3044e23fa3191338430e198315/.claude/skills/dynamic-instrumentation/SKILL.md) · 841★

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
