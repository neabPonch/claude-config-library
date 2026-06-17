---
name: DBraun__DawDreamer
source: https://github.com/DBraun/DawDreamer/blob/b891902bae3ef5cb9041373b888ceeb2a016f9d4/CLAUDE.md
repo: DBraun/DawDreamer
kind: claude-md
stars: 1246
last_pushed: 2026-02-07T03:43:51Z
license: gpl-3.0
score: 9
domains: [audio-engineering, python-dev]
tags: [build-instructions, multi-platform]
curated: 2026-06-14
curated_by: config-scout
---

# DBraun/DawDreamer — claude-md

**Why it's worth keeping:** Includes critical environment variables for architecture/path management and a troubleshooting table that pre-empts common build failures.

**Summary:** A highly specific, platform-aware guide for building a complex C++/Python audio framework with dependencies.

**Source credibility:** High; well-starred repository (1200+) used in professional audio contexts.

**Recency:** Current; supports modern Python versions and recent development workflows.

**Source:** [DBraun/DawDreamer/CLAUDE.md](https://github.com/DBraun/DawDreamer/blob/b891902bae3ef5cb9041373b888ceeb2a016f9d4/CLAUDE.md) · 1246★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# DawDreamer - LLM Quick Build & Install Guide

> **For architecture, development workflow, and detailed documentation, see [DEVELOPER.md](DEVELOPER.md)**

DawDreamer is a Digital Audio Workstation (DAW) framework for Python enabling programmatic audio processing with VST plugins, Faust DSP, and complex audio routing graphs.

**Python**: 3.11-3.14 | **License**: GPLv3

---

## Quick Install

`setup.py` handles the full flow: building C++ (if needed), copying the `.so`, and installing. It detects source changes and skips recompilation when up-to-date.

```bash
pip install -e .

# Verify
python3 -c "import dawdreamer; dawdreamer.RenderEngine(44100, 512)"
```

**WSL2 Note**: First install takes several minutes (C++ build + processing Faust libraries). Subsequent installs skip the C++ build if sources haven't changed.

---

## First-Time Setup (Prerequisites)

### Linux

```bash
# Install dependencies
sudo apt-get install -yq build-essential clang cmake git python3-dev \
  libboost-all-dev libfreetype6-dev libncurses-dev \
  libx11-dev libxrandr-dev libasound2-dev libxcomposite-dev

# Submodules and Faust
git submodule update --init --recursive
cd thirdparty/libfaust && python3 downloa
```

</details>
