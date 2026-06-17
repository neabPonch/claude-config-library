---
name: knova-run__sigil
source: https://github.com/knova-run/sigil/blob/48c5f70fd7408d282b42f54c6b3d4779c0079fec/CLAUDE.md
repo: knova-run/sigil
kind: claude-md
stars: 0
last_pushed: 2026-05-18T14:20:37Z
license: mit
score: 9
domains: [cli-tools, rust, code-analysis]
tags: [architecture-mapping, functional-structure, semantic-navigation]
curated: 2026-06-15
curated_by: config-scout
---

# knova-run/sigil — claude-md

**Why it's worth keeping:** The architecture section uses 'intent-based' grouping (e.g., 'Phase 1', 'Wiki-substrate') and embeds specific algorithm/logic details that allow an agent to understand *how* features work before reading the code.

**Summary:** This file provides a high-density functional map of the codebase, categorizing modules by their semantic role and logical phase rather than just listing files.

**Source credibility:** While the repo has low social proof (0 stars), the technical depth of the documentation suggests a sophisticated, high-complexity tool.

**Recency:** Highly current; it specifically targets 'Agent-facing' vs 'Script-facing' command surfaces.

**Source:** [knova-run/sigil/CLAUDE.md](https://github.com/knova-run/sigil/blob/48c5f70fd7408d282b42f54c6b3d4779c0079fec/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

sigil is a Rust CLI tool for structural code fingerprinting and diffing. It uses tree-sitter to parse source files, extract code entities (functions, classes, methods), compute content hashes, and produce entity-level diffs. Parsing and code-intelligence queries are fully in-house — no external indexer required.

## Build & Test

```bash
cargo build                          # default (lean) build
cargo build --features db,tokenizer  # full build: DuckDB backend + BPE tokenizer
cargo test                           # all tests
cargo test --lib                     # unit tests only
cargo test --test integration        # Index integration tests
cargo test --test diff_integration   # Diff integration tests
cargo test --test markdown_integration
```

## Architecture

```
src/
  lib.rs           — Library crate: re-exports modules for Python bindings and tests
  main.rs          — CLI binary (clap). Two-tier command surface:
                      Agent-facing: map, context, review, blast, benchmark
                      Script-facing: search, symbols, children, callers, callees,
                                     explore, duplicates, cochange, query, di
```

</details>
