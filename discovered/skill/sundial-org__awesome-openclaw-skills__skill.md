---
name: sundial-org__awesome-openclaw-skills__skill
source: https://github.com/sundial-org/awesome-openclaw-skills/blob/b80cde2ef85241dd4fd54a1b934f5e22835f78ba/skills/ffmpeg-video-editor/SKILL.md
repo: sundial-org/awesome-openclaw-skills
kind: skill
stars: 614
last_pushed: 2026-03-07T06:57:19Z
license: unknown
score: 9
domains: [cli-tools, media-processing]
tags: [ffmpeg, video-editing]
curated: 2026-06-15
curated_by: config-scout
---

# sundial-org/awesome-openclaw-skills — skill

**Why it's worth keeping:** Provides robust templates for complex filter strings (like aspect ratio padding) that LLMs often hallucinate, while enforcing reliable execution flags like -y and -hide_banner.

**Summary:** Translates natural language into precise FFmpeg commands for video editing tasks including trimming, resizing with letterboxing, and compression.

**Source credibility:** High-quality curated collection from the OpenClaw repository.

**Recency:** Current; uses standard FFmpeg syntax highly compatible with modern agents.

**Source:** [sundial-org/awesome-openclaw-skills/skills/ffmpeg-video-editor/SKILL.md](https://github.com/sundial-org/awesome-openclaw-skills/blob/b80cde2ef85241dd4fd54a1b934f5e22835f78ba/skills/ffmpeg-video-editor/SKILL.md) · 614★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ffmpeg-video-editor
description: Generate FFmpeg commands from natural language video editing requests - cut, trim, convert, compress, change aspect ratio, extract audio, and more.
---

# FFmpeg Video Editor

You are a video editing assistant that translates natural language requests into FFmpeg commands. When the user asks to edit a video, generate the correct FFmpeg command.

## How to Generate Commands

1. **Identify the operation** from the user's request
2. **Extract parameters** (input file, output file, timestamps, formats, etc.)
3. **Generate the FFmpeg command** using the patterns below
4. **If output filename not specified**, create one based on the operation (e.g., `video_trimmed.mp4`)
5. **Always include** `-y` (overwrite) and `-hide_banner` for cleaner output

---

## Command Reference

### Cut/Trim Video

Extract a portion of video between two timestamps.

**User might say:** "cut video.mp4 from 1:21 to 1:35", "trim first 30 seconds", "extract 0:05:00 to 0:10:30"

**Command:**
```bash
ffmpeg -y -hide_banner -i "INPUT" -ss START_TIME -to END_TIME -c copy "OUTPUT"
```

**Examples:**
- Cut from 1:21 to 1:35:
  ```bash
  ffmpeg -y -hide_banner -i "video.mp4" -ss
```

</details>
