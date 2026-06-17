---
name: camara-coder__talking-game
source: https://github.com/camara-coder/talking-game/blob/d2137a9c6b80308d87164c5b95d98f95bc0269c0/claude.md
repo: camara-coder/talking-game
kind: claude-md
stars: 0
last_pushed: 2026-03-09T21:59:20Z
license: unknown
score: 9
domains: [agents-ai, game-development, systems-architecture]
tags: [voice-agent, api-specification, multi-process]
curated: 2026-06-16
curated_by: config-scout
---

# camara-coder/talking-game — claude-md

**Why it's worth keeping:** The inclusion of exact API schemas, WebSocket event envelopes, and precise audio/protocol constraints provides an unambiguous blueprint that eliminates AI hallucination during implementation. It maps out the entire lifecycle of a user interaction across different running processes.

**Summary:** A highly detailed technical specification for a multi-process local voice agent system involving Unity, Python (FastAPI), and Ollama.

**Source credibility:** Single developer project; content demonstrates high technical density characteristic of real-world engineering work.

**Recency:** Very current (3 months ago) and utilizes modern voice-agent stacks like Pipecat and Kokoro.

**Source:** [camara-coder/talking-game/claude.md](https://github.com/camara-coder/talking-game/blob/d2137a9c6b80308d87164c5b95d98f95bc0269c0/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
\# Voice Conversational Kids Game (5+) — Windows CPU POC

\*\*Unity UI + Local Pipecat Voice Service + Ollama (LLM) + faster-whisper (STT) + Kokoro (TTS)\*\*



This document is a build-ready technical outline for a \*\*Windows PC proof-of-concept\*\*.  

Goal: a child presses a button, speaks into the mic, the game understands and responds out loud with \*\*short, simple\*\*, kid-friendly answers (and gets \*\*basic math\*\* correct).



---



\## 0) Summary of what you’re building



\### Runtime (local, on one Windows PC)

\- \*\*Unity Game (C#)\*\*: UI, character, captions, button, audio playback.

\- \*\*Voice Agent Service (Python)\*\*: Pipecat-driven pipeline (VAD → STT → Skills → LLM → TTS).

\- \*\*Ollama (local service)\*\*: hosts a small instruct LLM (CPU-friendly).

\- \*\*eSpeak NG\*\*: required dependency for Kokoro voice synthesis.



\### Key POC behaviors

\- \*\*Push-to-talk\*\* in Unity (simple turn-taking).

\- \*\*Deterministic math router\*\* (so “5 plus 5” always answers “10”).

\- \*\*Kid-mode prompt\*\* (1–2 short sentences; safe topics only).

\- \*\*Local-only\*\* execution after model downloads.



---



\## 1) Process layout (how programs run)



\###
```

</details>
