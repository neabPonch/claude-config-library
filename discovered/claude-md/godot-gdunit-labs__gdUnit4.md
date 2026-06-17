---
name: godot-gdunit-labs__gdUnit4
source: https://github.com/godot-gdunit-labs/gdUnit4/blob/612cf6b52df79f906d28e38987d9f3af17a21e97/CLAUDE.md
repo: godot-gdunit-labs/gdUnit4
kind: claude-md
stars: 1104
last_pushed: 2026-06-15T10:52:42Z
license: mit
score: 9
domains: [game-dev, cli-tools, testing-frameworks]
tags: [godot, gdscript, unit-testing, comprehensive]
curated: 2026-06-15
curated_by: config-scout
---

# godot-gdunit-labs/gdUnit4 — claude-md

**Why it's worth keeping:** Uses 'stop-and-tell' instructions for missing dependencies and detailed compatibility checks to prevent API misuse; employs a hierarchical documentation strategy (linking to test-specific CLAUDE.md).

**Summary:** A highly structured guide that provides specific execution commands, architecture mappings, and strict style enforcement rules.

**Source credibility:** Highly credible; well-maintained Godot engine plugin with significant community adoption.

**Recency:** Current; reflects modern Godot 4 / .NET development workflows and agentic coding needs.

**Source:** [godot-gdunit-labs/gdUnit4/CLAUDE.md](https://github.com/godot-gdunit-labs/gdUnit4/blob/612cf6b52df79f906d28e38987d9f3af17a21e97/CLAUDE.md) · 1104★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Project Is

GdUnit4 is a Godot 4 embedded unit testing framework (Godot plugin) supporting GDScript and C#.
The plugin lives entirely under `addons/gdUnit4/` and is self-tested — the framework uses itself to run its own test suite.

Supported Godot versions: (read the **Compatibility Overview** table in `README.md`
and find the row whose GdUnit4 version contains `master`). C# targets net9.0 with .NET SDK 9.0.308 (pinned in `global.json`).

## Commands

### Running Tests

Tests require a Godot binary. Set `GODOT_BIN` or pass `--godot_binary`:

```bash
# GDScript tests
export GODOT_BIN=/path/to/godot
./addons/gdUnit4/runtest.sh

# With explicit binary
./addons/gdUnit4/runtest.sh --godot_binary /path/to/godot

# Run a specific test path
./addons/gdUnit4/runtest.sh --godot_binary /path/to/godot -a res://addons/gdUnit4/test/asserts/
```

For .NET projects, `runtest.sh` also runs `dotnet build --debug` automatically.

### C# Build and Format

```bash
# Build
dotnet build --debug

# Verify formatting (CI-style check, no changes applied)
dotnet format gdUnit4.cs
```

</details>
