---
name: pktgen__Pktgen-DPDK
source: https://github.com/pktgen/Pktgen-DPDK/blob/f5f4ac0e84c74a7889f52dc1e0d16474d333c0b7/CLAUDE.md
repo: pktgen/Pktgen-DPDK
kind: claude-md
stars: 488
last_pushed: 2026-03-21T14:15:45Z
license: other
score: 10
domains: [cli-tools, networking, systems-programming]
tags: [c, dpdk, low-level, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# pktgen/Pktgen-DPDK — claude-md

**Why it's worth keeping:** It documents specific bitmask semantics, global state locations, and complex logic flows that an LLM cannot easily infer from code alone. This prevents 'logical hallucinations' when performing low-level systems programming.

**Summary:** Provides exhaustive build command mappings and deep architectural insights into internal state management and data flow.

**Source credibility:** High; the source is a well-known, active DPDK tool with strong community presence.

**Recency:** Very recent (3 months ago) and highly effective for modern agentic workflows.

**Source:** [pktgen/Pktgen-DPDK/CLAUDE.md](https://github.com/pktgen/Pktgen-DPDK/blob/f5f4ac0e84c74a7889f52dc1e0d16474d333c0b7/CLAUDE.md) · 488★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

---

## Build Commands

The project uses **Meson/Ninja**. A `builddir/` is typically already initialised.

```bash
# Incremental build (most common)
ninja -C builddir

# Full configure + build from scratch
meson setup builddir
meson compile -C builddir

# Makefile wrapper (delegates to tools/pktgen-build.sh)
make build          # release build
make rebuild        # clean + release build
make debug          # debug build (no optimisation)
make debugopt       # debug with -O2
make buildlua       # release + Lua scripting enabled
make clean

# Build options (pass to meson setup)
meson setup builddir -Denable_lua=true
meson setup builddir -Denable_docs=true
meson setup builddir -Donly_docs=true      # docs only, skip app/lib

# Code formatting
ninja -C builddir clang-format-check       # check only (CI does this)
ninja -C builddir clang-format             # auto-fix in place

# Documentation
make docs                                  # Sphinx + Doxygen

# Tests
ninja -C builddir test                     # meson test runner
# Integration tests are Lua scripts in test/ tha
```

</details>
