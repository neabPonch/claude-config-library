---
name: mbailey__voicemode
source: https://github.com/mbailey/voicemode/blob/585bbf8e5de668ea7b8949b4e764bc4289c6e9cf/CLAUDE.md
repo: mbailey/voicemode
kind: claude-md
stars: 1226
last_pushed: 2026-06-15T04:22:28Z
license: mit
score: 9
domains: [cli-tools, python, mcp-servers, automation]
tags: [release-management, architecture-overview, workflow-guidance]
curated: 2026-06-15
curated_by: config-scout
---

# mbailey/voicemode — claude-md

**Why it's worth keeping:** The 'Releases & Changelog' section is exceptional, teaching the agent exactly how to contribute without breaking CI/CD automation. It also includes specific toolchain requirements (uv, FFmpeg) and detailed component mapping.

**Summary:** Provides deep architectural context and exhaustive instructions for a high-stakes automated release workflow.

**Source credibility:** High; a popular (1200+ stars), actively maintained project with a clear development philosophy.

**Recency:** Extremely current, using modern tools like `uv` and providing up-to-date maintenance instructions.

**Source:** [mbailey/voicemode/CLAUDE.md](https://github.com/mbailey/voicemode/blob/585bbf8e5de668ea7b8949b4e764bc4289c6e9cf/CLAUDE.md) · 1226★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Voice Interaction

Load the voicemode skill for voice conversation support: `/voicemode:voicemode`

## Project Overview

VoiceMode is a Python package that provides voice interaction capabilities for AI assistants through the Model Context Protocol (MCP). It enables natural voice conversations with Claude Code and other AI coding assistants by integrating speech-to-text (STT) and text-to-speech (TTS) services.

## Key Commands

### Development & Testing
```bash
# Install in development mode with dependencies
make dev-install

# Run all unit tests
make test
# Or directly: uv run pytest tests/ -v --tb=short

# Run specific test
uv run pytest tests/test_voice_mode.py -v

# Clean build artifacts
make clean
```

### Building & Publishing
```bash
# Build Python package
make build-package

# Build development version (auto-versioned)
make build-dev  

# Test package installation
make test-package

# Release workflow (bumps version, tags, pushes) — see "Releases & Changelog" below before running
make release
```

### Documentation
```bash
# Serve docs locally at http://lo
```

</details>
