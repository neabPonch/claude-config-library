---
name: alexkapoulas__BiomePruner
source: https://github.com/alexkapoulas/BiomePruner/blob/d10bbe2b50e9249741be291c2a1a5fc5be35d6f3/CLAUDE.md
repo: alexkapoulas/BiomePruner
kind: claude-md
stars: 0
last_pushed: 2025-07-23T23:30:45Z
license: gpl-3.0
score: 9
domains: [game-dev, java, cli-tools]
tags: [automation, workflow, wrapper-scripts]
curated: 2026-06-14
curated_by: config-scout
---

# alexkapoulas/BiomePruner — claude-md

**Why it's worth keeping:** Uses the 'wrapper script' pattern to prevent agent errors (e.g., 'Never run gradle directly') and provides clear instructions for automated validation/log parsing.

**Summary:** Provides a highly structured workflow using specialized Python command wrappers to abstract complex build, test, and log analysis tasks.

**Source credibility:** Low social proof (0 stars), but demonstrates sophisticated project-specific tooling logic.

**Recency:** Extremely current, referencing very recent Minecraft/NeoForge versions.

**Source:** [alexkapoulas/BiomePruner/CLAUDE.md](https://github.com/alexkapoulas/BiomePruner/blob/d10bbe2b50e9249741be291c2a1a5fc5be35d6f3/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Development Guide

## Project Information

- **Minecraft Version**: 1.21.1
- **NeoForge Version**: 21.1.193
- **Parchment Mappings**: 2024.11.17 (MC 1.21.1)

## Development Workflow

### 1. After Making Source Code Changes
**Always validate your changes with the build script:**
```bash
python claude_tooling/scripts/build_script.py
```
- Exit code 0 = success, continue with your task
- Exit code 1 = build failed, check `claude_tooling/build_output/` for error reports
- Fix errors and repeat until build succeeds

### 2. Testing and Debugging
**When you need to test mod functionality or debug issues:**
```bash
python claude_tooling/scripts/run_automated_tests.py
```
- Runs comprehensive automated tests including biome replacement and performance tests
- Generates detailed reports in `claude_tooling/test_output/`
- Includes automatic log parsing and error extraction

### 3. Configuration Management
**When you need to modify mod settings:**
```bash
python claude_tooling/scripts/config_manager.py read general microBiomeThreshold
python claude_tooling/scripts/config_manager.py write general microBiomeThreshold 75
```
- Safe access to mod configuration (excludes protected tes
```

</details>
