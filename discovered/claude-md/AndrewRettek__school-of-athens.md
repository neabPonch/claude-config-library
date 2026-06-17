---
name: AndrewRettek__school-of-athens
source: https://github.com/AndrewRettek/school-of-athens/blob/db925748c29641cc21a0b3642a11eeb630803324/CLAUDE.md
repo: AndrewRettek/school-of-athens
kind: claude-md
stars: 0
last_pushed: 2026-05-07T19:29:29Z
license: unknown
score: 9
domains: [game-dev, fullstack-web, ai-integration]
tags: [renpy, flask, procedural-assets, checklist]
curated: 2026-06-15
curated_by: config-scout
---

# AndrewRettek/school-of-athens — claude-md

**Why it's worth keeping:** The 'Self-Review Checklist' translates domain expertise into actionable guardrails, while the 'Adding a New Character' section provides a perfect procedural recipe for LLM execution.

**Summary:** This file provides deep architectural context for a Ren'Py engine and Flask backend, including specific initialization orders and asset generation workflows. It features an exceptional self-review checklist targeting niche engine-specific pitfalls.

**Source credibility:** Low social proof (0 stars) but contains high-density technical detail characteristic of an actual developer.

**Recency:** Current; explicitly references Claude Code functionality.

**Source:** [AndrewRettek/school-of-athens/CLAUDE.md](https://github.com/AndrewRettek/school-of-athens/blob/db925748c29641cc21a0b3642a11eeb630803324/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

School of Athens — a Ren'Py phone-texting simulator where players chat with ancient Greek philosophers (Socrates, Aristotle, Heraclitus, Epicurus, Herodotus, Diogenes) powered by DeepInfra AI (DeepSeek V3) via a Flask proxy server. Resolution is 1280x720 with a warm marble & gold visual theme.

## Architecture

### Two-Part System

1. **Ren'Py Game Client** (`game/`) — The visual novel, a phone UI with chat screens. Uses `renpy.fetch()` for non-blocking HTTP and `renpy.invoke_in_thread()` for background API calls.
2. **Flask Proxy Server** (`server/app.py`) — Deployed separately (Railway). Holds the DeepInfra API key server-side, validates player tokens, rate-limits requests, forwards chat completions. Currently open (auth decorator exists but is not applied to `/v1/chat`).

### Game Code Flow

- `script.rpy` — State machine loop. `phone_state` toggles between `"messages"`, `"contacts"`, and `"chat"`. Uses `call screen` pattern (screens return `(action, data)` tuples via `Return()`).
- `characters.rpy` — System prompts + `ChatSession` instances.
```

</details>
