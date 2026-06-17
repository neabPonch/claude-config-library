---
name: skaggsxyz__moltstream
source: https://github.com/skaggsxyz/moltstream/blob/c521f9cff19833ed4f4ef6bdf69bf3c6a3049d09/skill.md
repo: skaggsxyz/moltstream
kind: skill
stars: 68
last_pushed: 2026-04-09T21:24:57Z
license: mit
score: 8
domains: [agents-ai, streaming-media, mcp-servers, automation]
tags: [streaming, kick, mcp, voice-tts, avatar]
curated: 2026-06-15
curated_by: config-scout
---

# skaggsxyz/moltstream — skill

**Why it's worth keeping:** Demonstrates a perfect pattern for documenting MCP server installation and tool availability; provides a clear bridge between LLM reasoning and complex multimedia execution.

**Summary:** Provides an agent-native runtime for conducting live streams on Kick with integrated TTS, avatar animation, and OBS control. It includes ready-to-use MCP server integration for direct tool access by Claude/Cursor.

**Source credibility:** Solid niche project with moderate star count and recent activity.

**Recency:** Highly current, specifically utilizing the Model Context Protocol (MCP) standard.

**Source:** [skaggsxyz/moltstream/skill.md](https://github.com/skaggsxyz/moltstream/blob/c521f9cff19833ed4f4ef6bdf69bf3c6a3049d09/skill.md) · 68★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: moltstream
description: >
  AI agent-native streaming runtime for Kick. Use MoltStream to build agents
  that operate live streams — react to chat, generate voiced responses, animate
  avatars with lip sync, and broadcast to Kick via OBS. One command to go live.
capabilities:
  - kick-streaming
  - chat-reaction
  - tts-voice-synthesis
  - avatar-lip-sync
  - obs-integration
  - scene-composition
  - reasoning-trace-logging
  - character-generation
context_cost: 500
ttfa_minutes: 3
min_context_window: 8000
auth: api-key
---

# MoltStream Skill

## What you can do
- Deploy an AI-powered live stream on Kick with one command
- React to viewer chat in real-time via LLM (Gemini / Claude)
- Generate voiced responses (Fish Audio / ElevenLabs / OpenAI)
- Animate an avatar with lip sync and chat overlay
- Compose scenes declaratively (video, overlays, audio)
- Enforce content policies and safety guardrails
- Log every decision as a structured reasoning trace
- Generate AI characters from photos (Gemini Vision + Imagen)

## Quick start
```bash
npx moltstream init     # configure your agent
npx moltstream start    # go live on Kick
npx moltstream mcp      # start MCP server for Clau
```

</details>
