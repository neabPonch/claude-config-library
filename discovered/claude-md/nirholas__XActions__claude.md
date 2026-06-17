---
name: nirholas__XActions__claude
source: https://github.com/nirholas/XActions/blob/3f20f4b05541cb7aa86d9f4a951f771b7661ee2f/xspace-agents/CLAUDE.md
repo: nirholas/XActions
kind: claude-md
stars: 310
last_pushed: 2026-05-07T05:10:46Z
license: other
score: 9
domains: [agents-ai, automation, cli-tools, typescript]
tags: [monorepo, architecture, agentic-workflow, puppeteer]
curated: 2026-06-15
curated_by: config-scout
---

# nirholas/XActions — claude-md

**Why it's worth keeping:** Includes highly specific environmental hacks (terminal killing) and provides the AI with a mental model of complex logic flows through ASCII diagrams and class tables.

**Summary:** A high-density architectural guide featuring class-to-file mappings, detailed data flow sequences, and monorepo organization.

**Source credibility:** Strong; 310 stars and actively maintained open-source project.

**Recency:** Current and perfectly optimized for modern LLM/Claude Code workflows.

**Source:** [nirholas/XActions/xspace-agents/CLAUDE.md](https://github.com/nirholas/XActions/blob/3f20f4b05541cb7aa86d9f4a951f771b7661ee2f/xspace-agents/CLAUDE.md) · 310★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — xspace-agent Monorepo

**Kill every terminal** — always use `isBackground: true`, then kill the terminal after output is captured

## What This Project Is

**xspace-agent** is a TypeScript SDK and CLI that enables AI agents to autonomously join, listen, and speak in X (Twitter) Spaces. It supports multiple LLM providers (OpenAI, Claude, Groq), speech-to-text (Whisper), text-to-speech (ElevenLabs, OpenAI TTS), and multi-agent coordination — all driven by Puppeteer browser automation against the live X Spaces UI.

**Target**: Open-source developer tool. Proprietary (All Rights Reserved). Published to npm as `xspace-agent` (core SDK), `@xspace/server` (admin panel), `@xspace/cli` (CLI).

## Monorepo Layout

```
packages/
  core/          → xspace-agent         Main SDK. XSpaceAgent class, providers, audio, browser automation, FSM, intelligence layer.
  server/        → @xspace/server       Express + Socket.IO admin panel with auth, rate limiting, real-time agent control.
  cli/           → @xspace/cli          CLI tool (xspace-agent init|auth|join|start|dashboard).
  widget/        → UI widget components (early stage).
  create-xspace-agent/ → Project scaffolding templat
```

</details>
