---
name: Zackriya-Solutions__meetily
source: https://github.com/Zackriya-Solutions/meetily/blob/0281737d87d26352fb0adc78c8c0975f691b23d1/CLAUDE.md
repo: Zackriya-Solutions/meetily
kind: claude-md
stars: 12729
last_pushed: 2026-06-05T13:53:17Z
license: mit
score: 9
domains: [desktop-app, rust, audio-processing]
tags: [architectural-mapping, ipc-patterns, module-routing]
curated: 2026-06-15
curated_by: config-scout
---

# Zackriya-Solutions/meetily — claude-md

**Why it's worth keeping:** It maps error types to specific file paths and provides exact code examples for the Frontend-to-Backend communication interface, minimizing AI guesswork.

**Summary:** Provides deep technical context for a Tauri/Rust desktop app, specifically detailing complex audio processing pipelines and cross-language IPC patterns.

**Source credibility:** High; comes from a highly-starred (12k+) active open-source project.

**Recency:** Very current; references Tauri 2.x and Next.js 14.

**Source:** [Zackriya-Solutions/meetily/CLAUDE.md](https://github.com/Zackriya-Solutions/meetily/blob/0281737d87d26352fb0adc78c8c0975f691b23d1/CLAUDE.md) · 12729★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Meetily** is a privacy-first AI meeting assistant that captures, transcribes, and summarizes meetings entirely on local infrastructure. The supported application is the Tauri desktop app with a Rust core.

1. **Frontend**: Tauri-based desktop application (Rust + Next.js + TypeScript)
2. **Rust Backend**: Tauri commands, audio capture, transcription, storage, and summarization orchestration
3. **Legacy Backend Archive**: the old Python/FastAPI, Docker, and standalone whisper-server backend under `backend/` is archived and unsupported

### Key Technology Stack
- **Desktop App**: Tauri 2.x (Rust) + Next.js 14 + React 18
- **Audio Processing**: Rust (cpal, whisper-rs, professional audio mixing)
- **Transcription**: Whisper.cpp / whisper-rs and Parakeet paths in the Tauri app
- **App API Surface**: Tauri commands and events, not a separate FastAPI service
- **LLM Integration**: Ollama (local), Claude, Groq, OpenRouter

## Essential Development Commands

### Frontend Development (Tauri Desktop App)

**Location**: `/frontend`

```bash
# macOS Developm
```

</details>
