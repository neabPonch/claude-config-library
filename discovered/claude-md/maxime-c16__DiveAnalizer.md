---
name: maxime-c16__DiveAnalizer
source: https://github.com/maxime-c16/DiveAnalizer/blob/05bf12825e3f92e8da55b6cce7c3637a8fb479c9/CLAUDE.md
repo: maxime-c16/DiveAnalizer
kind: claude-md
stars: 0
last_pushed: 2026-01-24T09:14:29Z
license: unknown
score: 9
domains: [computer-vision, python, cli-tools]
tags: [line-indexing, state-machine, architectural-context, command-reference]
curated: 2026-06-16
curated_by: config-scout
---

# maxime-c16/DiveAnalizer — claude-md

**Why it's worth keeping:** It utilizes exact line-number indexing for navigating large files, explains complex logic via state machine transitions, and provides implementation templates for extending functionality.

**Summary:** A high-density technical guide that includes an ongoing architectural roadmap, detailed command patterns, and a breakdown of internal state machines.

**Source credibility:** Single developer repository with high technical depth in the documentation provided.

**Recency:** Highly current; includes modern multi-modal AI/CV integration details.

**Source:** [maxime-c16/DiveAnalizer/CLAUDE.md](https://github.com/maxime-c16/DiveAnalizer/blob/05bf12825e3f92e8da55b6cce7c3637a8fb479c9/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Architecture Overhaul in Progress

**See `ARCHITECTURE_PLAN.md` for the complete v2.0 redesign plan.**

The project is transitioning from a MediaPipe-based visual splash detection system to a multi-modal approach using:
- Audio peak detection (librosa) - primary signal
- Motion burst detection (Decord + frame diff) - validation
- YOLO-nano person detection - validation
- FFmpeg stream copy extraction - instant clip export

## Project Overview

DiveAnalyzer is an automated diving video analysis tool that uses computer vision and AI to detect and extract individual dives from swimming pool diving videos. It combines MediaPipe pose detection, OpenCV computer vision, and multiple splash detection algorithms in a state machine architecture.

## Development Commands

### Running the Main Application

```bash
# Basic usage with default settings (motion_intensity splash detection)
python3 slAIcer.py path/to/video.mp4

# With custom output directory
python3 slAIcer.py video.mp4 --output_dir extracted_dives

# Enable debug visualization window (helpful for tuning detection
```

</details>
