---
name: elizaOS__eliza__skill
source: https://github.com/elizaOS/eliza/blob/0250bfb980773163ae408a606fda100dd2f0e895/packages/benchmarks/skillsbench/tasks/mario-coin-counting/environment/skills/ffmpeg/SKILL.md
repo: elizaOS/eliza
kind: skill
stars: 18581
last_pushed: 2026-06-14T21:48:59Z
license: mit
score: 8
domains: [cli-tools, media-processing]
tags: [ffmpeg, video, keyframes]
curated: 2026-06-15
curated_by: config-scout
---

# elizaOS/eliza — skill

**Why it's worth keeping:** It distinguishes between high-control filter methods and high-performance skip-frame methods, including essential flags like -q:v and -vsync vfr.

**Summary:** Provides optimized FFmpeg command patterns for extracting I-frames (keyframes) from various video formats.

**Source credibility:** High; sourced from elizaOS, a highly-starred and actively maintained agentic framework.

**Recency:** Current; uses standard CLI utilities applicable to modern environments.

**Source:** [elizaOS/eliza/packages/benchmarks/skillsbench/tasks/mario-coin-counting/environment/skills/ffmpeg/SKILL.md](https://github.com/elizaOS/eliza/blob/0250bfb980773163ae408a606fda100dd2f0e895/packages/benchmarks/skillsbench/tasks/mario-coin-counting/environment/skills/ffmpeg/SKILL.md) · 18581★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ffmpeg-keyframe-extraction
description: Extract key frames (I-frames) from video files using FFmpeg command line tool. Use this skill when the user needs to pull out keyframes, thumbnails, or important frames from MP4, MKV, AVI, or other video formats for analysis, previews, or processing.
license: Complete terms in LICENSE.txt
---

# FFmpeg Keyframe Extraction

Extract key frames (I-frames) from video files using FFmpeg CLI.

## Prerequisites

- FFmpeg installed and available in PATH
- Input video file (MP4, MKV, AVI, MOV, etc.)

## Methods

### Method 1: Select Filter (More Control)

```bash
ffmpeg -i <input_video> -vf "select='eq(pict_type,I)'" -vsync vfr <output_pattern>
Method 2: Skip Frame (Faster)

ffmpeg -skip_frame nokey -i <input_video> -vsync vfr <output_pattern>
Key Options
Option	Description
-i <file>	Input video file
-vf "select='eq(pict_type,I)'"	Filter selecting only I-frames
-skip_frame nokey	Skip decoding non-keyframes (performance)
-vsync vfr	Variable frame rate, prevents duplicates
-q:v <n>	Quality (1-31, lower = better, for JPEG)
-frame_pts 1	Use presentation timestamp in filename
Output Patterns
frame_%03d.png - PNG sequence (frame_001.png, frame_002
```

</details>
