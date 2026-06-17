---
name: IanTrudel__Glyph
source: https://github.com/IanTrudel/Glyph/blob/039ab3fbedebaa300edb3bf6f53093e65768ec5b/CLAUDE.md
repo: IanTrudel/Glyph
kind: claude-md
stars: 0
last_pushed: 2026-04-08T07:32:39Z
license: other
score: 9
domains: [cli-tools, compilers, systems-programming]
tags: [toolchain, language-specification, technical-reference]
curated: 2026-06-15
curated_by: config-scout
---

# IanTrudel/Glyph — claude-md

**Why it's worth keeping:** The exhaustive CLI command reference and explicit compilation pipelines allow an LLM to operate with high autonomy without needing to guess syntax or tool capabilities.

**Summary:** A highly detailed technical manual for a unique SQLite-based programming language that covers the entire build/bootstrap lifecycle.

**Source credibility:** High technical complexity; likely written by a systems engineer/compiler architect.

**Recency:** Very recent (2 months ago), fully optimized for modern agentic coding workflows.

**Source:** [IanTrudel/Glyph/CLAUDE.md](https://github.com/IanTrudel/Glyph/blob/039ab3fbedebaa300edb3bf6f53093e65768ec5b/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Glyph is an LLM-native programming language where **programs are SQLite3 databases** (`.glyph` files), not source files. The unit of storage is the *definition*, and SQL queries replace the traditional module/import system. The language is designed for token-minimal syntax to minimize BPE token count for LLM generation and consumption.

**Current status:** Working compiler. Two compilers exist:
- **Self-hosted compiler** (`glyph.glyph` → `./glyph`): ~1,774 definitions (1,399 fn + 360 test + 13 type + 2 const), C codegen backend with monomorphization, LLVM IR backend (`--emit=llvm`), 30 CLI commands, MCP server. This is the primary compiler.
- **Rust compiler** (`cargo run -- ...`): Cranelift backend, used as bootstrap tool (`glyph0`) to rebuild `glyph.glyph`.

## Build Commands

### Bootstrap chain (build the self-hosted compiler)

```bash
ninja                          # full bootstrap: glyph0 → glyph
ninja test                     # run all tests (Rust + self-hosted)
```

### Rust compiler (bootstrap tool)

```bash
cargo build
```

</details>
