---
name: mahmoudimus__static_asm
source: https://github.com/mahmoudimus/static_asm/blob/ee0005ea96f133792bfc9f757b7890f273a73773/CLAUDE.md
repo: mahmoudimus/static_asm
kind: claude-md
stars: 31
last_pushed: 2026-01-26T20:01:39Z
license: other
score: 9
domains: [systems-programming, cpp]
tags: [cmake, c++20, x86]
curated: 2026-06-15
curated_by: config-scout
---

# mahmoudimus/static_asm — claude-md

**Why it's worth keeping:** Provides a concrete 'Usage Pattern' code snippet and a clear step-by-step workflow for extending the library, which is vital for autonomous maintenance tasks.

**Summary:** Defines build commands, architectural components, and namespace mappings for a C++20 compile-time assembler.

**Source credibility:** Specialized niche library with high-quality documentation and recent activity.

**Recency:** Current; reflects modern C++20/2x development standards.

**Source:** [mahmoudimus/static_asm/CLAUDE.md](https://github.com/mahmoudimus/static_asm/blob/ee0005ea96f133792bfc9f757b7890f273a73773/CLAUDE.md) · 31★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build Commands

```bash
# Configure (from repo root)
cmake -B build -DCMAKE_BUILD_TYPE=Release

# Build
cmake --build build -j$(nproc)

# Run all tests
ctest --test-dir build --output-on-failure

# Run a single test (by name pattern)
ctest --test-dir build -R "AdcInstructions" --output-on-failure

# Build with examples (requires Clang, uses inline assembly)
cmake -B build -DCMAKE_BUILD_TYPE=Release -DSTATIC_ASM_BUILD_EXAMPLES=ON
```

## Architecture

This is a **header-only C++20 library** for compile-time x86 assembly encoding. All code executes at compile time using `consteval` functions.

### Key Components

- **`include/static_asm.hpp`** - Main include file (amalgamated header)
- **`include/static_asm/core.hpp`** - `assemble()` and `emit()` functions (emit requires Clang/GCC with -O2)

### x86 Encoding Layer (`include/static_asm/x86/`)

- **`operands.hpp`** - Register, immediate, and memory operand types with C++20 concepts
- **`encoder.hpp`** - Instruction encoding functions (`encode_alu`, `encode_mov`, `encode_jmp`, etc.)
- **`gen/instruction.g.hpp`** - High
```

</details>
