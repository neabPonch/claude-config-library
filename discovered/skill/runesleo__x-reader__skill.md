---
name: runesleo__x-reader__skill
source: https://github.com/runesleo/x-reader/blob/6085af9568f14f2e944c41703342133deca54776/skills/video/skill.md
repo: runesleo/x-reader
kind: skill
stars: 945
last_pushed: 2026-05-31T14:57:15Z
license: mit
score: 9
domains: [media-processing, automation-agents, web-scraping]
tags: [multimedia, transcription, yt-dlp, automation]
curated: 2026-06-15
curated_by: config-scout
---

# runesleo/x-reader — skill

**Why it's worth keeping:** Demonstrates advanced tool-use techniques like bypassing platform restrictions (Bilibili API/Referer headers) and implementing audio segmentation to handle API payload limits.

**Summary:** A sophisticated multi-step pipeline that automates media extraction (video/audio), transcription via Groq's Whisper, and structured summarization.

**Source credibility:** High; 945 stars on a specialized media extraction repo indicates a proven, community-vetted utility.

**Recency:** Extremely current; utilizes high-speed models like whisper-large-v3-turbo and modern yt-dlp workflows.

**Source:** [runesleo/x-reader/skills/video/skill.md](https://github.com/runesleo/x-reader/blob/6085af9568f14f2e944c41703342133deca54776/skills/video/skill.md) · 945★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Video & Podcast Digest Skill

> Send a video/podcast link → get full transcript + structured summary

## Supported Platforms

| Platform | Type | Subtitles | Whisper Transcription |
|----------|------|-----------|----------------------|
| YouTube | Video | ✅ | ✅ |
| Bilibili | Video | ✅ | ✅ |
| X/Twitter | Video | ❌ | ✅ |
| Xiaoyuzhou (小宇宙) | Podcast | ❌ | ✅ |
| Apple Podcasts | Podcast | ❌ | ✅ |
| Direct links (mp3/mp4/m3u8) | Any | ❌ | ✅ |

## Trigger

Auto-triggered when a media URL is detected:
- YouTube: `youtube.com`, `youtu.be`
- Bilibili: `bilibili.com`, `b23.tv`
- X/Twitter: `x.com`, `twitter.com` (tweets with video)
- Xiaoyuzhou: `xiaoyuzhoufm.com`
- Apple Podcasts: `podcasts.apple.com`
- Direct: `.mp3`, `.mp4`, `.m3u8`, `.m4a`, `.webm`

## Pipeline

### Step 0: Detect Media Type

| URL Pattern | Type | Pipeline |
|-------------|------|----------|
| `xiaoyuzhoufm.com/episode/` | Podcast | → Step 1b (Xiaoyuzhou) |
| `podcasts.apple.com` | Podcast | → Step 1c (Apple) |
| `bilibili.com`, `b23.tv` | Video | → Step 1d (Bilibili API) |
| `.mp3`, `.m4a` direct link | Audio | → Step 2b (direct download) |
| Other | Video | → Step 1a (subtitle extraction) |

### Step 1a: Video —
```

</details>
