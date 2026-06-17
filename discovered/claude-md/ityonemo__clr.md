---
name: ityonemo__clr
source: https://github.com/ityonemo/clr/blob/168a3716f758979bea832aab269a1a555f9c7d0d/CLAUDE.md
repo: ityonemo/clr
kind: claude-md
stars: 235
last_pushed: 2026-06-06T16:38:55Z
license: mit
score: 9
domains: [systems-programming, compiler-engineering, cli-tools]
tags: [zig, testing-workflows, debugging, build-system]
curated: 2026-06-15
curated_by: config-scout
---

# ityonemo/clr — claude-md

**Why it's worth keeping:** Includes 'CRITICAL' behavioral constraints to prevent the AI from modifying tests to pass, and provides an efficient loop for debugging generated code artifacts.

**Summary:** Provides hyper-specific build/test instructions and a rigorous debugging workflow for a custom compiler plugin. It emphasizes exact command usage to avoid environmental issues.

**Source credibility:** Strong; 235 stars and very recent maintenance indicates a high-quality repository.

**Recency:** Highly current; includes advanced workflow patterns relevant to Claude Code's agentic capabilities.

**Source:** [ityonemo/clr/CLAUDE.md](https://github.com/ityonemo/clr/blob/168a3716f758979bea832aab269a1a555f9c7d0d/CLAUDE.md) · 235★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLR Project

## Project Structure

- `zig/` - Zig compiler submodule (DO NOT MODIFY - all changes must be non-AI)

## Build Commands

- `zig/b` - Builds the custom Zig compiler (uses `zig build --zig-lib-dir lib`)
- `zig/z` - Runs the custom Zig compiler from `zig-out/bin/zig`
- `zig build -Doptimize=ReleaseFast` - Builds libclr.so (the AIR plugin) **IMPORTANT: Always use ReleaseFast unless you need to do advanced debugging and you have recompiled Zig to be in a different mode**
- `zig build test` - Runs unit tests for libclr
- `./run_integration.sh` - Runs BATS integration tests
- `./run_one.sh <test_file>` - Run a single test case (generates `.air.zig` file in project root)
- `./dump_air.sh <source_file> <function_name> [num_lines]` - Dump AIR for a specific function
- `./clear.sh` - Clean up generated `.air.zig` files and other build artifacts

### Debugging AIR

To view the raw AIR for a function:
```sh
./dump_air.sh test/cases/undefined/basic/assigned_before_use.zig assigned_before_use.main 40
```

This shows the instruction indices, tags, and nesting structure. Block bodies may have indices that are **higher** than post-block instructions (e.g., block at %10 may contain %16
```

</details>
