---
name: chipsalliance__Surelog
source: https://github.com/chipsalliance/Surelog/blob/65a98524782971ac81c43286a173c39b6bc09edb/CLAUDE.md
repo: chipsalliance/Surelog
kind: claude-md
stars: 463
last_pushed: 2026-05-31T17:33:48Z
license: apache-2.0
score: 9
domains: [compilers, cli-tools, systems-programming]
tags: [systemverilog, compiler, build-system]
curated: 2026-06-15
curated_by: config-scout
---

# chipsalliance/Surelog — claude-md

**Why it's worth keeping:** The 'ScratchPad Test' section provides a perfect example of high-value context: a specific, heavy-duty debug command to verify changes. The architecture breakdown also maps directory structures to functional logic, which is critical for LLM navigation.

**Summary:** Provides a deep architectural map and precise command-line interfaces for building, testing, and debugging a complex SystemVerilog compiler.

**Source credibility:** High; sourced from Chips Alliance, a professional organization maintaining critical industry infrastructure.

**Recency:** Current; includes highly detailed toolchain and debugging workflows suitable for modern agentic coding.

**Source:** [chipsalliance/Surelog/CLAUDE.md](https://github.com/chipsalliance/Surelog/blob/65a98524782971ac81c43286a173c39b6bc09edb/CLAUDE.md) · 463★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Surelog is a SystemVerilog 2017 pre-processor, parser, elaborator, and UHDM compiler. It provides IEEE Design/TB C/C++ VPI and Python AST APIs for use by linters, simulators, synthesis tools, and formal verification tools.

## Build Commands

### Primary Build Commands
```bash
# Standard release build
make -j$(nproc)

# Debug build
make debug

# Release build with Python support
make release_with_python

# Release build without tcmalloc (for compatibility)
make release_no_tcmalloc

# Shared library build
make release-shared

# Clean build artifacts
make clean

# Install to system (default: /usr/local)
make install
# Custom prefix: PREFIX=/path/to/install make install
```

### Testing Commands
```bash
# Run unit tests
make test/unittest

# Run regression tests
make test/regression

# Run both unit and regression tests  
make test

# Run tests in parallel with custom options
cd build && tclsh ../tests/regression.tcl diff_mode show_diff

# Run specific test
cd build && ../bin/surelog ../tests/<TestName>/dut.sv

# Run valgrind memory checks
make test
```

</details>
