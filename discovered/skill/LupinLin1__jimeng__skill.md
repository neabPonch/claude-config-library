---
name: LupinLin1__jimeng__skill
source: https://github.com/LupinLin1/jimeng/blob/1b69411fe4f07b9ccf7bc655a780ad6aaf32a088/jimeng-api/Skill.md
repo: LupinLin1/jimeng
kind: skill
stars: 24
last_pushed: 2026-05-02T16:39:28Z
license: gpl-3.0
score: 8
domains: [agents-ai, cli-tools, media-generation]
tags: [image-generation, video-generation, async-tasks, api-integration]
curated: 2026-06-15
curated_by: config-scout
---

# LupinLin1/jimeng — skill

**Why it's worth keeping:** It demonstrates excellent patterns for stateful session management (saving Session IDs) and handling asynchronous task workflows. The 'Parameter Discipline' and troubleshooting sections are highly transferable templates for any custom tool integration.

**Summary:** A specialized skill for interacting with the Jimeng AI API to generate images and videos via a CLI.

**Source credibility:** Moderate; a small-scale reverse-engineered project with active recent updates.

**Recency:** Highly relevant for modern agentic coding environments that require specialized CLI tools.

**Source:** [LupinLin1/jimeng/jimeng-api/Skill.md](https://github.com/LupinLin1/jimeng/blob/1b69411fe4f07b9ccf7bc655a780ad6aaf32a088/jimeng-api/Skill.md) · 24★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: jimeng-api
description: >
  Generate images and videos using the Jimeng API (即梦AI) at jimeng.modelhub.cc.
  Use this skill when users request AI-generated images, artwork, illustrations,
  or AI-generated videos from the Jimeng service. Supports text-to-image,
  image-to-image, text-to-video, image-to-video (first frame), first+last frame,
  and omni_reference video generation (with mixed image/video/audio materials).
  Default image model: jimeng-5.0. Video models: jimeng-video-seedance-2.0 / 2.0-fast.
  Video generation is always async: submit task → receive task_id.
compatibility: "python>=3.7, requests>=2.28.0, Pillow>=9.0.0"
---

# Jimeng API

## Overview

This skill generates images and videos via the Jimeng API at `https://jimeng.modelhub.cc`.
Images are downloaded immediately; videos are async (submit → poll separately).

## Session ID

**Session ID is required for every call.**

### First time in a conversation

Ask the user:

> "请提供您的 Session ID（从即梦网站 Cookie 中获取 sessionid）。
> 如果使用国际站，请加对应前缀：us- / hk- / jp- / sg-"

Region prefixes:
- 国内站: no prefix
- 美国站: `us-`
- 香港/日本/新加坡: `hk-` / `jp-` / `sg-`

### Save and reuse

**Once the user provides their Session ID, save
```

</details>
