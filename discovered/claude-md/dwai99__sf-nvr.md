---
name: dwai99__sf-nvr
source: https://github.com/dwai99/sf-nvr/blob/7eb57b0dec3c14db0b10317da240c2a45e7e7be4/CLAUDE.md
repo: dwai99/sf-nvr
kind: claude-md
stars: 0
last_pushed: 2026-06-13T03:52:46Z
license: unknown
score: 8
domains: [backend, web-development, video-processing]
tags: [nvr, ffmpeg, flask, media-server]
curated: 2026-06-16
curated_by: config-scout
---

# dwai99/sf-nvr — claude-md

**Why it's worth keeping:** Includes highly practical 'when to restart' logic and preventative troubleshooting tips for common time-handling and video-sync bugs.

**Summary:** Provides system architecture, deployment workflows, and critical domain-specific technical constraints for a video recording system.

**Source credibility:** Low star count but the content is highly structured and professional.

**Recency:** 

**Source:** [dwai99/sf-nvr/CLAUDE.md](https://github.com/dwai99/sf-nvr/blob/7eb57b0dec3c14db0b10317da240c2a45e7e7be4/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# NVR Project

Network Video Recorder system with web-based playback and live viewing.

## Quick Start

```bash
# Server management
./start.sh      # Start the server
./stop.sh       # Stop the server
./restart.sh    # Restart the server

# Run tests
pytest

# Run specific test file
pytest tests/test_file.py -v
```

## Architecture

```
nvr/
├── app.py              # Flask application entry point
├── core/
│   ├── recorder.py     # Camera recording logic
│   ├── transcoder.py   # FFmpeg video processing
│   ├── motion.py       # Motion detection
│   ├── playback_db.py  # Recording segment database
│   └── recording_modes.py  # Schedule-based recording
├── web/
│   ├── api.py          # Main API endpoints
│   ├── playback_api.py # Playback/streaming endpoints
│   └── recording_api.py # Recording mode endpoints
├── templates/
│   ├── index.html      # Live view page
│   ├── playback.html   # Playback page (complex - has timeline, seeking, multi-camera sync)
│   └── settings.html   # Settings page
└── static/
    ├── notifications.js
    ├── timeline-selector.js
    └── ui-utils.js
```

## Key Technical Details

### Video Pipeline
- Cameras accessed via RTSP
- FFmpeg handles recording
```

</details>
