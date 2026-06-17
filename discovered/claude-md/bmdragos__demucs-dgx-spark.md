---
name: bmdragos__demucs-dgx-spark
source: https://github.com/bmdragos/demucs-dgx-spark/blob/d0342a207cf8f3024c3326b9093406bdffeba275/claude.md
repo: bmdragos/demucs-dgx-spark
kind: claude-md
stars: 1
last_pushed: 2026-01-13T20:27:55Z
license: mit
score: 8
domains: [backend-api, machine-learning, infrastructure]
tags: [audio-processing, fastapi, nvidia-dgx]
curated: 2026-06-15
curated_by: config-scout
---

# bmdragos/demucs-dgx-spark — claude-md

**Why it's worth keeping:** Uses structured tables for rapid endpoint/parameter lookups and explicitly defines critical system-level CLI commands (DGX MCP) for agentic environment control.

**Summary:** A high-density technical specification for an audio processing server, covering architecture, model parameters, and API routes.

**Source credibility:** Niche repository with low star count; likely a specialized engineering tool.

**Recency:** Highly current with modern AI-driven development workflows.

**Source:** [bmdragos/demucs-dgx-spark/claude.md](https://github.com/bmdragos/demucs-dgx-spark/blob/d0342a207cf8f3024c3326b9093406bdffeba275/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# DJ Gizmo

AI-powered audio processing server for DJ/remix applications. Runs on DGX Spark (GB10 GPU, 128GB unified memory).

## What This Is

A FastAPI server that provides:
- **Stem separation** - Split songs into drums, bass, other, vocals (~30s)
- **Sound effect generation** - Text-to-audio via Stable Audio Open (~1s small, ~65s full)
- **Audio analysis** - BPM, key, beats, onsets, segments, waveforms
- **Rendering** - Time-stretch, pitch-shift, cut stems on demand

## Architecture

```
server.py          # FastAPI server, job queues, all endpoints
index.html         # Web UI (drag-drop upload, real-time status)
setup.sh           # Surgical install script for NGC containers
stable-audio.md    # Model documentation for Stable Audio Open
```

## Key Technical Details

- **Container:** `nvcr.io/nvidia/pytorch:25.12-py3` on DGX Spark
- **Models:** Demucs htdemucs, Stable Audio Open (small + full)
- **Job queues:** Async queues for separation and effect generation
- **Analysis:** Parallel via ProcessPoolExecutor (5 workers)
- **Output:** 44.1kHz stereo WAV

## API Endpoints

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/separate` | POST | Upload file,
```

</details>
