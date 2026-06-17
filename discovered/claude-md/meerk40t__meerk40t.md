---
name: meerk40t__meerk40t
source: https://github.com/meerk40t/meerk40t/blob/d55c43c7d7c64067ee7f97873045fcec8f624a7a/CLAUDE.md
repo: meerk40t/meerk40t
kind: claude-md
stars: 399
last_pushed: 2026-06-10T16:02:30Z
license: mit
score: 9
domains: [cli-tools, hardware-control, python]
tags: [plugin-architecture, event-driven, systems-programming]
curated: 2026-06-15
curated_by: config-scout
---

# meerk40t/meerk40t — claude-md

**Why it's worth keeping:** Explicitly defines the custom Signal vs Channel event systems to prevent AI hallucinations of standard event patterns. The inclusion of plugin lifecycles and a detailed node-tree hierarchy makes it highly actionable for adding new features.

**Summary:** A high-density development guide that explains complex architectural patterns and internal communication protocols.

**Source credibility:** High; the repository is actively maintained with recent commits and significant community interest (399 stars).

**Recency:** Very current; includes modern Python toolchain commands and up-to-date project status.

**Source:** [meerk40t/meerk40t/CLAUDE.md](https://github.com/meerk40t/meerk40t/blob/d55c43c7d7c64067ee7f97873045fcec8f624a7a/CLAUDE.md) · 399★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - MeerK40t Development Guide

## Project Overview

MeerK40t (pronounced "MeerKat") is an open-source laser cutting/engraving control software. It provides a highly extensible, plugin-based platform supporting multiple laser hardware types including K40 (Lihuiyu), GRBL, Ruida, Moshiboard, Newly, and galvo (Balor) lasers.

**Version:** 0.9.9000 (Active Development)
**License:** MIT
**Python:** 3.6+
**Platforms:** Windows, macOS, Linux, Raspberry Pi

See `NOTES.md` for current device stability status. See `.github/copilot-instructions.md` for an additional development reference.

---

## Quick Commands

```bash
# Install with all features
pip install meerk40t[all]

# Run application
python -m meerk40t              # Full GUI
python -m meerk40t --no-gui     # Console mode
python -m meerk40t --simpleui   # Simplified interface

# Run tests
python -m unittest discover test -v
pytest -v

# Code quality
flake8 meerk40t test
black --check meerk40t test
mypy meerk40t
```

---

## Architecture

### Plugin-Based System

Everything is a plugin with lifecycle phases:
```
plugins → preregister → register → configure → boot → postboot → start
```

Standard plugin pattern:
```python
def
```

</details>
