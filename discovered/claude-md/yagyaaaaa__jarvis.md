---
name: yagyaaaaa__jarvis
source: https://github.com/yagyaaaaa/jarvis/blob/781244f334d640d061714dd3411d7b1fa67a1081/CLAUDE.md
repo: yagyaaaaa/jarvis
kind: claude-md
stars: 0
last_pushed: 2026-03-21T00:39:50Z
license: unknown
score: 7
domains: [agents-ai, cli-tools]
tags: [voice-ai, local-llm, cuda, low-latency]
curated: 2026-06-15
curated_by: config-scout
---

# yagyaaaaa/jarvis — claude-md

**Why it's worth keeping:** It includes domain-specific architectural constraints regarding latency minimization and CUDA error patterns, plus an actionable task list to guide multi-session development.

**Summary:** Establishes operational context for a low-latency local voice AI system emphasizing hardware interaction and model orchestration.

**Source credibility:** Low social proof (0 stars) but contains highly specialized technical instructions typical of a reference implementation.

**Recency:** Highly current; relevant to modern local LLM/hardware orchestration workflows.

**Source:** [yagyaaaaa/jarvis/CLAUDE.md](https://github.com/yagyaaaaa/jarvis/blob/781244f334d640d061714dd3411d7b1fa67a1081/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Guidelines - Jarvis Framework

This document provides context and standards for Claude Code to maintain and evolve the Jarvis local-first AI assistant.

## Project Vision
A modular, high-performance, and privacy-centric AI agent. Goal: Orchestrate disparate local models (Whisper, Kokoro, Mistral) into a seamless, low-latency loop.

## Development Commands
- **Install Dependencies:** `pip install -r requirements.txt`
- **Run Application:** `python src/main.py` (or use `run.bat` for Windows)
- **Test GPU/CUDA:** `python test_gpu.py`
- **Model Downloader:** `python download_model.py`

## Project Structure & Architecture
- `src/`: Core logic for the agent loop and state management.
- `tools/`: Utility scripts for OpenCV vision processing and math.
- `config/`: YAML-based configuration for model paths and hardware settings.
- `data/vectorstore/`: RAG storage for long-term assistant memory.

## Coding Standards
- **Performance First:** Minimize latency between STT (Whisper) and TTS (Kokoro). Use asynchronous processing where possible.
- **Error Handling:** Implement robust logging (referencing `jarvis_crash.log` patterns) for hardware-specific failures (OOM, CUDA errors).
-
```

</details>
