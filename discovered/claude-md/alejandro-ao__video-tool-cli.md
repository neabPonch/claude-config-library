---
name: alejandro-ao__video-tool-cli
source: https://github.com/alejandro-ao/video-tool-cli/blob/642f156887657936101c40af480b830fa2db6275/CLAUDE.md
repo: alejandro-ao/video-tool-cli
kind: claude-md
stars: 16
last_pushed: 2026-06-02T15:08:08Z
license: unknown
score: 9
domains: [cli-tools, media-processing, python]
tags: [cli, video, ffmpeg, mixins]
curated: 2026-06-16
curated_by: config-scout
---

# alejandro-ao/video-tool-cli — claude-md

**Why it's worth keeping:** The architectural breakdown describes exactly what each module does within the 'VideoProcessor' pattern, and the Environment section prevents trial-and-error by specifying how to manage API keys/OAuth rather than just using env vars.

**Summary:** This file maps a complex mixin-based architecture and provides an exhaustive list of CLI commands for both operation and system configuration. It clearly explains how the project handles sensitive credentials and environment setup via dedicated CLI commands.

**Source credibility:** A small but active repository utilizing modern toolchains like uv.

**Recency:** Highly current; uses latest Python standards (3.11+) and modern package management practices.

**Source:** [alejandro-ao/video-tool-cli/CLAUDE.md](https://github.com/alejandro-ao/video-tool-cli/blob/642f156887657936101c40af480b830fa2db6275/CLAUDE.md) · 16★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
# Install (dev)
uv tool install --editable .

# Run CLI
video-tool --help
video-tool video concat --help

# Tests
pytest                              # all tests
pytest -m "unit and not slow"       # fast unit tests
pytest --cov=video_tool --cov=main  # with coverage
```

## Architecture

**Entry points**: `main.py` → `video_tool/cli` package (interactive CLI commands)

**VideoProcessor (mixin pattern)** in `video_tool/video_processor/`:
- `base.py`: Core config, LLM clients (OpenAI/Groq via native SDKs), loguru logging
- `concatenation.py`: ffmpeg video joining, fast concat, timestamp generation
- `content.py`: Description, SEO, social posts, context cards (uses prompts.yaml)
- `transcript.py`: Groq Whisper transcription
- `deployment.py`: Bunny.net CDN uploads
- `youtube.py`: YouTube API uploads (OAuth2)
- `processor.py`: Facade composing all mixins

**CLI commands** (all support interactive prompts when args omitted):
- Video: `download`, `silence-removal`, `concat`, `timestamps`, `extract-audio`, `enhance-audio`, `replace-audio`, `info`, `tri
```

</details>
