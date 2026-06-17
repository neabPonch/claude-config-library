---
name: kittynXR__apnger
source: https://github.com/kittynXR/apnger/blob/3106ae6303e0464c799c5e3cabcf27a141057d65/CLAUDE.md
repo: kittynXR/apnger
kind: claude-md
stars: 2
last_pushed: 2026-01-28T23:13:46Z
license: mit
score: 9
domains: [desktop-app, video-processing, electron]
tags: [ffmpeg, ipc, media-encoding]
curated: 2026-06-16
curated_by: config-scout
---

# kittynXR/apnger — claude-md

**Why it's worth keeping:** It documents complex FFmpeg filter math (frame sampling/palette generation) and exact IPC communication mappings, which prevents AI hallucination of prohibited browser-side Node calls.

**Summary:** An exceptionally detailed guide for an Electron-based video processing tool that bridges technical architecture with domain-specific media logic.

**Source credibility:** Low star count but the extreme specificity of the technical implementation details suggests a high-quality, specialized tool.

**Recency:** Very current; references modern versions like React 19 and Vite 7.

**Source:** [kittynXR/apnger/CLAUDE.md](https://github.com/kittynXR/apnger/blob/3106ae6303e0464c799c5e3cabcf27a141057d65/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Apnger is a cross-platform desktop application (Electron + React + TypeScript) that converts video files with transparent or chroma-keyed backgrounds into optimized emotes for multiple platforms: Twitch, Discord (stickers and emotes), and 7TV. The application features a GUI with drag-and-drop support, real-time chroma key preview, and one-click export to all formats.

## Architecture

### Tech Stack
- **Desktop Framework**: Electron 38+
- **Frontend**: React 19 + TypeScript 5
- **Build Tool**: Vite 7
- **State Management**: Zustand
- **Video Processing**: FFmpeg 8.0 (bundled native binaries)
- **Bundler**: electron-builder
- **Distribution**: Portable executable with zero external dependencies

### Project Structure

```
apnger/
├── src/
│   ├── main/              # Electron main process
│   │   ├── main.ts        # App entry, window management, IPC handlers, FFmpeg path resolution
│   │   └── preload.ts     # Secure IPC bridge to renderer
│   ├── renderer/          # React frontend
│   │   ├── App.tsx        # Main app component
│   │   ├── main
```

</details>
