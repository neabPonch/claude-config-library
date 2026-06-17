---
name: SharpAI__DeepCamera__skill
source: https://github.com/SharpAI/DeepCamera/blob/2264fcb20e545a8bc5b41097494e93b776104bf3/skills/streaming/go2rtc-cameras/SKILL.md
repo: SharpAI/DeepCamera
kind: skill
stars: 2833
last_pushed: 2026-04-21T19:30:51Z
license: mit
score: 7
domains: [security, iot, media-streaming]
tags: [RTSP, WebRTC, go2rtc, camera-management]
curated: 2026-06-15
curated_by: config-scout
---

# SharpAI/DeepCamera — skill

**Why it's worth keeping:** Demonstrates efficient parameterization using dense string entries and provides the exact JSONL protocol for agent-to-service IPC communication.

**Summary:** Configures go2rtc to translate multiple RTSP streams into low-latency WebRTC web views via a specific skill script.

**Source credibility:** High; highly starred, specialized AI/Vision repository with recent activity.

**Recency:** Current; follows modern agentic tool-calling and sidecar service patterns.

**Source:** [SharpAI/DeepCamera/skills/streaming/go2rtc-cameras/SKILL.md](https://github.com/SharpAI/DeepCamera/blob/2264fcb20e545a8bc5b41097494e93b776104bf3/skills/streaming/go2rtc-cameras/SKILL.md) · 2833★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: go2rtc-cameras
description: "Multi-camera RTSP to WebRTC streaming via go2rtc"
version: 1.0.0

parameters:
  - name: streams
    label: "RTSP Stream URLs"
    type: string
    description: "Comma-separated camera_name=rtsp://... entries"
    placeholder: "front_door=rtsp://192.168.1.100:554/stream1"
    required: true
    group: Streams

capabilities:
  live_stream:
    script: scripts/stream.py
    description: "Register RTSP streams with go2rtc for WebRTC playback"
---

# go2rtc Multi-Camera Streaming

Registers RTSP camera streams with SharpAI Aegis's go2rtc sidecar for low-latency WebRTC live view in the browser.

## How It Works

```
Your Cameras (RTSP)          go2rtc (in Aegis)           Browser
───────────────────          ─────────────────           ───────
rtsp://cam1:554/stream ───►  /api/webrtc?src=cam1  ───► WebRTC Player
rtsp://cam2:554/stream ───►  /api/webrtc?src=cam2  ───► WebRTC Player
rtsp://cam3:554/stream ───►  /api/webrtc?src=cam3  ───► WebRTC Player
```

## Supported Sources

go2rtc accepts any stream source:
- `rtsp://` — standard RTSP cameras
- `rtmp://` — RTMP streams
- `http://` — MJPEG or HLS streams
- `ffmpeg:` — FFmpeg pipeline
- `exec:` — cu
```

</details>
