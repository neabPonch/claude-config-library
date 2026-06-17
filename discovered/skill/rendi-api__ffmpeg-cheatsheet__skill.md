---
name: rendi-api__ffmpeg-cheatsheet__skill
source: https://github.com/rendi-api/ffmpeg-cheatsheet/blob/a9de5b10448b6b6bc59671d347691bdcd5c34be8/skills/ffmpeg/SKILL.md
repo: rendi-api/ffmpeg-cheatsheet
kind: skill
stars: 1715
last_pushed: 2026-04-29T19:44:19Z
license: unknown
score: 9
domains: [cli-tools, media-automation]
tags: [ffmpeg, video, audio, conversion]
curated: 2026-06-15
curated_by: config-scout
---

# rendi-api/ffmpeg-cheatsheet — skill

**Why it's worth keeping:** The 'Workflow' section establishes logic instead of just commands, and the 'Gotchas' effectively prevent common AI errors like inaccurate trimming or playback incompatibility.

**Summary:** Provides a structured mental model for media automation using FFmpeg, covering conversion, filtering, and stream mapping.

**Source credibility:** High; 1700+ stars indicates a widely-used community resource.

**Recency:** Current; provides modern standards for H.264/H.265 and web compatibility.

**Source:** [rendi-api/ffmpeg-cheatsheet/skills/ffmpeg/SKILL.md](https://github.com/rendi-api/ffmpeg-cheatsheet/blob/a9de5b10448b6b6bc59671d347691bdcd5c34be8/skills/ffmpeg/SKILL.md) · 1715★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ffmpeg
description: >
  Use when the user asks for FFmpeg or FFprobe commands, video/audio conversion,
  trimming, resizing, padding, overlays, subtitles, thumbnails, GIFs, storyboards,
  slideshows, social-media crops, codec settings, CRF/preset tuning, stream mapping,
  or troubleshooting media automation pipelines.
---

# FFmpeg

Use this skill to produce reliable, explainable FFmpeg/FFprobe commands for media automation.

## Workflow

1. Identify the user's source media, desired output container/codec, target dimensions/duration, and whether quality, speed, or file size matters most.
2. Prefer the simplest command that meets the goal.
3. Use `-c copy` only when no filtering, re-encoding, precise trimming, subtitle burn-in, compression, or codec change is needed.
4. Use explicit stream mapping when multiple inputs or outputs are involved.
5. For commands with filters, quote the filter graph and name streams in `filter_complex` when it improves readability.
6. Include `-y` only when the user wants non-interactive overwrite behavior.
7. Validate command intent with `ffprobe` or a low-duration sample when practical.

## Defaults

- Web-compatible MP4: `-c:v libx264 -crf 1
```

</details>
