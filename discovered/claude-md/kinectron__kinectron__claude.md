---
name: kinectron__kinectron__claude
source: https://github.com/kinectron/kinectron/blob/18dfb5600104389e93a68438d13b87d8ce3c4500/.claude/claude.md
repo: kinectron/kinectron
kind: claude-md
stars: 333
last_pushed: 2026-05-22T21:26:00Z
license: mit
score: 9
domains: [hardware-integration, web-streaming, electron-app]
tags: [iot, webrtc, monorepo, computer-vision]
curated: 2026-06-16
curated_by: config-scout
---

# kinectron/kinectron — claude-md

**Why it's worth keeping:** Includes high-value 'gotchas' like manual DLL/ONNX file copies, specific implementation patterns for new streams, and instructions to use the internal debugging system over console.log.

**Summary:** Provides deep architectural context for a hardware-to-web streaming system, detailing how data flows from Azure Kinect to browsers via WebRTC.

**Source credibility:** Strong; 333 stars indicates a used tool with detailed, expert-level technical documentation.

**Recency:** Current; uses modern monorepo (npm workspaces) and development workflows relevant to contemporary AI coding agents.

**Source:** [kinectron/kinectron/.claude/claude.md](https://github.com/kinectron/kinectron/blob/18dfb5600104389e93a68438d13b87d8ce3c4500/.claude/claude.md) · 333★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Kinectron Project Context

## Overview
Kinectron streams Microsoft Azure Kinect data to web browsers via WebRTC. It's an Electron desktop app (server) + JavaScript client library (browser) that enables creative coders, researchers, and interactive designers to access depth-sensing data in web applications.

**Current Status**: Version 1.0.0 - All streams implemented and working

## Architecture

```
Azure Kinect Hardware
  → KinectController (app/main)
  → Stream Processors (app/main/processors)
  → Stream Handlers (app/main/handlers)
  → PeerConnectionManager (WebRTC)
  → Kinectron Client API (browser)
  → Web Applications
```

### Components
- **App (`app/`)**: Electron application (Windows only, requires Azure Kinect SDK)
  - Main process: Kinect interface, stream processing, WebRTC server
  - Renderer process: UI, peer connection UI
- **Client (`client/`)**: Browser JavaScript library (cross-platform dev)
  - Multi-format build: ESM, CJS, UMD
  - WebRTC peer connection via PeerJS
  - Stream handlers for all data types

## Tech Stack
- **Electron**: Desktop app framework
- **PeerJS/WebRTC**: Real-time browser communication
- **Azure Kinect SDK**: Native hardware interface (Win
```

</details>
