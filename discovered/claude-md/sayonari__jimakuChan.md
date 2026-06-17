---
name: sayonari__jimakuChan
source: https://github.com/sayonari/jimakuChan/blob/7084ad3007c67fa49f94f4893838b63f73cd5fa0/CLAUDE.md
repo: sayonari/jimakuChan
kind: claude-md
stars: 70
last_pushed: 2026-03-05T13:24:50Z
license: mit
score: 8
domains: [web-frontend, speech-recognition]
tags: [constraints, architecture-guide, visual-rendering]
curated: 2026-06-15
curated_by: config-scout
---

# sayonari/jimakuChan — claude-md

**Why it's worth keeping:** Includes high-value 'CRITICAL DEVELOPMENT RULES' that explicitly prevent the agent from executing server startup commands or committing code without manual user verification.

**Summary:** Provides detailed architectural context and specific technical nuances for a custom text rendering system and SSL/Web Speech API requirements.

**Source credibility:** Solid; 70-star project with recent maintenance history.

**Recency:** Current; utilizes specific behavioral constraints relevant to Claude Code's tool-use capabilities.

**Source:** [sayonari/jimakuChan/CLAUDE.md](https://github.com/sayonari/jimakuChan/blob/7084ad3007c67fa49f94f4893838b63f73cd5fa0/CLAUDE.md) · 70★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

- セッション開始時に共通ルールである、AGENTS.mdを必ず読み込むこと。
- 読み込んだことを最初に報告すること
- 以下は Claude Code固有の差分のみ記載する

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

jimakuChan (音声認識字幕ちゃん) is a real-time speech recognition and translation subtitle application for streamers and content creators. The application provides live subtitles with multi-language translation support and customizable visual styling.

## Architecture

The application consists of three main components:

1. **Configuration Interface** (`index.html`) - A comprehensive settings panel where users configure:
   - Speech recognition language settings
   - Translation target languages (up to 3 simultaneous translations)
   - Visual styling (fonts, colors, borders, sizes)
   - Google Translate API integration
   - Bouyomi-chan TTS integration

2. **Subtitle Display** (`main.html`) - The actual subtitle overlay that:
   - Performs real-time speech recognition using Web Speech API
   - Displays recognized text with visual effects (stroke, colors, positioning)
   - Handles translation via Google Translate API
   - Supports multiple simultaneous translation outp
```

</details>
