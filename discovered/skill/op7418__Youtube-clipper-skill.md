---
name: op7418__Youtube-clipper-skill
source: https://github.com/op7418/Youtube-clipper-skill/blob/f31f077ee0905c95a510a6f34bbd0c3c85b15129/SKILL.md
repo: op7418/Youtube-clipper-skill
kind: skill
stars: 1954
last_pushed: 2026-01-22T04:56:21Z
license: mit
score: 9
domains: [cli-tools, video-processing, automation]
tags: [youtube, ffmpeg, ai-analysis]
curated: 2026-06-14
curated_by: config-scout
---

# op7418/Youtube-clipper-skill — skill

**Why it's worth keeping:** Includes expert technical instructions like environment dependency verification (FFmpeg/libass), handling shell path spacing issues via temporary directories, and optimizing API calls through batch translation logic.

**Summary:** A comprehensive workflow for transforming long YouTube videos into structured, translated, and captioned short clips using AI-driven semantic analysis.

**Source credibility:** High community validation with nearly 2k stars and recent updates.

**Recency:** Current; maintains highly relevant tool-use patterns for Claude Code.

**Source:** [op7418/Youtube-clipper-skill/SKILL.md](https://github.com/op7418/Youtube-clipper-skill/blob/f31f077ee0905c95a510a6f34bbd0c3c85b15129/SKILL.md) · 1954★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: youtube-clipper
description: >
  YouTube 视频智能剪辑工具。下载视频和字幕，AI 分析生成精细章节（几分钟级别），
  用户选择片段后自动剪辑、翻译字幕为中英双语、烧录字幕到视频，并生成总结文案。
  使用场景：当用户需要剪辑 YouTube 视频、生成短视频片段、制作双语字幕版本时。
  关键词：视频剪辑、YouTube、字幕翻译、双语字幕、视频下载、clip video
allowed-tools:
  - Read
  - Write
  - Bash
  - Glob
  - AskUserQuestion
model: claude-sonnet-4-5-20250514
---

# YouTube 视频智能剪辑工具

> **Installation**: If you're installing this skill from GitHub, please refer to [README.md](README.md#installation) for installation instructions. The recommended method is `npx skills add https://github.com/op7418/Youtube-clipper-skill`.

## 工作流程

你将按照以下 6 个阶段执行 YouTube 视频剪辑任务：

### 阶段 1: 环境检测

**目标**: 确保所有必需工具和依赖都已安装

1. 检测 yt-dlp 是否可用
   ```bash
   yt-dlp --version
   ```

2. 检测 FFmpeg 版本和 libass 支持
   ```bash
   # 优先检查 ffmpeg-full（macOS）
   /opt/homebrew/opt/ffmpeg-full/bin/ffmpeg -version

   # 检查标准 FFmpeg
   ffmpeg -version

   # 验证 libass 支持（字幕烧录必需）
   ffmpeg -filters 2>&1 | grep subtitles
   ```

3. 检测 Python 依赖
   ```bash
   python3 -c "import yt_dlp; print('✅ yt-dlp available')"
   python3 -c "import pysrt; print('✅ pysrt available')"
   ```

**如果环境检测失败**:
- yt-dlp 未安装: 提示 `brew install yt-dlp` 或 `pip install yt-dlp`
- FFmpeg 无
```

</details>
