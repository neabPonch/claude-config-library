---
name: lucemia__typed-ffmpeg__skill
source: https://github.com/lucemia/typed-ffmpeg/blob/83def952ee0e3f8d92fcf11b54ae7681e5358b88/.claude/skills/typed-ffmpeg-usage/SKILL.md
repo: lucemia/typed-ffmpeg
kind: skill
stars: 1156
last_pushed: 2026-06-12T22:09:07Z
license: mit
score: 8
domains: [cli-tools, media-processing, python]
tags: [ffmpeg, video-editing, type-safe]
curated: 2026-06-16
curated_by: config-scout
---

# lucemia/typed-ffmpeg — skill

**Why it's worth keeping:** Provides high-value patterns for partial evaluation (reusable filter functions) and command compilation that allow an agent to build modular processing pipelines.

**Summary:** A comprehensive technical guide for the typed-ffmpeg library covering stream manipulation, complex filter graphs, and media probing.

**Source credibility:** Strong; highly starred repository with recent maintenance.

**Recency:** Current; utilizes modern Python type hinting and library structures.

**Source:** [lucemia/typed-ffmpeg/.claude/skills/typed-ffmpeg-usage/SKILL.md](https://github.com/lucemia/typed-ffmpeg/blob/83def952ee0e3f8d92fcf11b54ae7681e5358b88/.claude/skills/typed-ffmpeg-usage/SKILL.md) · 1156★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: typed-ffmpeg-usage
description: Guide for using typed-ffmpeg, a modern Python FFmpeg wrapper with extensive typing support and comprehensive filter support. Use this when working with FFmpeg operations, video/audio processing, or filter graphs in Python.
license: MIT
metadata:
  author: lucemia
  version: "1.0"
  compatibility: Python 3.10+
---

# typed-ffmpeg Usage Skill

This skill provides comprehensive guidance for using the **typed-ffmpeg** package, a modern Python FFmpeg wrapper that emphasizes type safety, IDE integration, and comprehensive filter support.

## Package Overview

**typed-ffmpeg** is a zero-dependency Python library (pure standard library) that provides:
- Extensive support for FFmpeg filters with detailed typing and documentation
- Full IDE auto-completion and type checking
- Filter graph visualization and serialization
- Media file analysis (ffprobe integration)
- Input/output options support
- Partial evaluation for modular filter construction

## Installation

```bash
# Basic installation
pip install typed-ffmpeg

# With graph visualization support
pip install 'typed-ffmpeg[graph]'

# For compatibility with ffmpeg-python
pip install typed-ffmpeg-c
```

</details>
