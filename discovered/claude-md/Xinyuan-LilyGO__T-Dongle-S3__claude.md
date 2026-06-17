---
name: Xinyuan-LilyGO__T-Dongle-S3__claude
source: https://github.com/Xinyuan-LilyGO/T-Dongle-S3/blob/fda1b85f75851e6dea66a5eb35f8d8e1bafcebea/lib/FastLED/CLAUDE.md
repo: Xinyuan-LilyGO/T-Dongle-S3
kind: claude-md
stars: 379
last_pushed: 2026-04-24T08:30:54Z
license: mit
score: 8
domains: [embedded-systems, cli-tools, ci-cd]
tags: [hierarchical-context, esp32, uv, automation]
curated: 2026-06-15
curated_by: config-scout
---

# Xinyuan-LilyGO/T-Dongle-S3 — claude-md

**Why it's worth keeping:** The modular 'index-to-subfolder' pattern is highly scalable for large repos; includes strict, environment-specific command patterns like forcing 'uv run'.

**Summary:** Uses a hierarchical structure where the root file acts as an index to specialized AGENTS.md files in subdirectories.

**Source credibility:** LilyGO is a reputable hardware developer; repository shows recent activity.

**Recency:** Very current, utilizing modern toolchains like uv and mentioning MCP servers.

**Source:** [Xinyuan-LilyGO/T-Dongle-S3/lib/FastLED/CLAUDE.md](https://github.com/Xinyuan-LilyGO/T-Dongle-S3/blob/fda1b85f75851e6dea66a5eb35f8d8e1bafcebea/lib/FastLED/CLAUDE.md) · 379★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# FastLED AI Agent Guidelines

## Quick Reference

This project uses directory-specific agent guidelines. See:

- **CI/Build Tasks**: `ci/AGENTS.md` - Python build system, compilation, MCP server tools
- **Testing**: `tests/AGENTS.md` - Unit tests, test execution, validation requirements  
- **Examples**: `examples/AGENTS.md` - Arduino sketch compilation, .ino file rules

## Key Commands

- `uv run test.py` - Run all tests
- `uv run test.py --cpp` - Run C++ tests only
- `uv run test.py TestName` - Run specific C++ test (e.g., `uv run test.py xypath`)
- `bash lint` - Run code formatting/linting
- `uv run ci/ci-compile.py uno --examples Blink` - Compile examples for specific platform
- `uv run ci/wasm_compile.py examples/Blink --just-compile` - Compile Arduino sketches to WASM
- `uv run mcp_server.py` - Start MCP server for advanced tools

### QEMU Commands
- `uv run ci/install-qemu.py` - Install QEMU for ESP32 emulation (standalone)
- `uv run test.py --qemu esp32s3` - Run QEMU tests (installs QEMU automatically)
- `FASTLED_QEMU_SKIP_INSTALL=true uv run test.py --qemu esp32s3` - Skip QEMU installation step

## Core Rules

### Command Execution (ALL AGENTS)
- **Python**: Always use `u
```

</details>
