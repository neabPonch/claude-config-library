---
name: giongto35__cloud-morph
source: https://github.com/giongto35/cloud-morph/blob/9bb2e0648f19cfa11fabc8dfb4f69abee299740a/CLAUDE.md
repo: giongto35/cloud-morph
kind: claude-md
stars: 1170
last_pushed: 2026-02-26T15:32:58Z
license: mit
score: 8
domains: [systems, streaming, backend]
tags: [webrtc, go, docker, low-latency]
curated: 2026-06-15
curated_by: config-scout
---

# giongto35/cloud-morph — claude-md

**Why it's worth keeping:** The use of text-based data flow diagrams (video/audio/input) and the breakdown of containerized processes provides vital context for debugging low-level system interactions.

**Summary:** Explains a complex WebRTC streaming architecture involving Go, Wine, and FF-mpeg with detailed data flow paths.

**Source credibility:** High; a popular open-source project with significant stars and recent activity.

**Recency:** Current; includes specific profiling and local development instructions.

**Source:** [giongto35/cloud-morph/CLAUDE.md](https://github.com/giongto35/cloud-morph/blob/9bb2e0648f19cfa11fabc8dfb4f69abee299740a/CLAUDE.md) · 1170★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

CloudMorph is a decentralized, self-hosted cloud gaming/application platform that streams Windows applications to web browsers via WebRTC. It virtualizes Windows apps using Wine in Docker containers and streams video/audio with ultra-low latency.

## Common Commands

```bash
# Setup (installs Docker, Go, builds Wine container)
./setup.sh

# Run the server (starts Go server + Docker container)
go run server.go

# Access at http://localhost:8080
# Profiling at http://localhost:3535/debug/pprof

# Run without Docker (debug mode) — requires modifying server.go to use run-wine-nodocker.sh
```

There are no automated tests in this project.

## Architecture

**Data flow:**
```
Browser ←WebRTC(video/audio)→ Go Server ←TCP:9090/UDP:5004,4004→ Docker Container (Wine+FFmpeg+syncinput)
Browser ←WebSocket(input/ctrl)→ Go Server
```

**Video/Audio output:** Wine app → Xvfb virtual display → FFmpeg (x11grab + PulseAudio) → RTP → Go server → WebRTC → browser

**Input path:** Browser → WebSocket → Go server → TCP:9090 → syncinput.exe (C++ WinAPI input injector ru
```

</details>
