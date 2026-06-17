---
name: nirholas__xspace-AI
source: https://github.com/nirholas/xspace-AI/blob/eb1810830097b1dda53e51d2408d9a308dbc51e2/CLAUDE.md
repo: nirholas/xspace-AI
kind: claude-md
stars: 15
last_pushed: 2026-05-17T17:30:50Z
license: other
score: 9
domains: [agents-ai, typescript-monorepo, cli-tools]
tags: [architecture-map, workflow-constraints, mental-model]
curated: 2026-06-15
curated_by: config-scout
---

# nirholas/xspace-AI — claude-md

**Why it's worth keeping:** Uses detailed technical diagrams and 'Key Class' tables to build a mental model; includes high-stakes operational instructions (git flags/terminal killing) that prevent common automation errors.

**Summary:** Provides comprehensive architectural maps, class mappings, and critical workflow caveats like specific git identity constraints and production deployment warnings.

**Source credibility:** Moderate; 15 stars with very recent activity indicates an active, well-maintained tool.

**Recency:** Highly current, utilizing modern patterns suitable for agentic workflows.

**Source:** [nirholas/xspace-AI/CLAUDE.md](https://github.com/nirholas/xspace-AI/blob/eb1810830097b1dda53e51d2408d9a308dbc51e2/CLAUDE.md) · 15★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — xspace-agent Monorepo

**Kill every terminal** — always use `isBackground: true`, then kill the terminal after output is captured

## Git Identity
Always commit and push as nirholas. Use these flags on every `git commit`:
```
git -c user.name="nirholas" -c user.email="22895867+nirholas@users.noreply.github.com" commit ...
```
Never use a different author. The Co-Authored-By trailer should also use this identity.

## What This Project Is

**xspace-agent** is a TypeScript SDK and CLI that enables AI agents to autonomously join, listen, and speak in X (Twitter) Spaces. It supports multiple LLM providers (OpenAI, Claude, Groq), speech-to-text (Whisper), text-to-speech (ElevenLabs, OpenAI TTS), and multi-agent coordination — all driven by Puppeteer browser automation against the live X Spaces UI.

**Target**: Open-source developer tool. Proprietary (All Rights Reserved). Published to npm as `xspace-agent` (core SDK), `@xspace/server` (admin panel), `@xspace/cli` (CLI).

## Monorepo Layout

```
packages/
  core/          → xspace-agent         Main SDK. XSpaceAgent class, providers, audio, browser automation, FSM, intelligence layer.
  server/        → @xspace/server
```

</details>
