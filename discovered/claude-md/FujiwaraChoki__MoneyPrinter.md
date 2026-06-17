---
name: FujiwaraChoki__MoneyPrinter
source: https://github.com/FujiwaraChoki/MoneyPrinter/blob/2a7c6bc6e8fab6e01fa740c4311d9e1e233b0262/CLAUDE.md
repo: FujiwaraChoki/MoneyPrinter
kind: claude-md
stars: 13527
last_pushed: 2026-03-26T22:17:17Z
license: mit
score: 9
domains: [media-automation, backend-api, ai-agents]
tags: [pipeline-heavy, comprehensive]
curated: 2026-06-15
curated_by: config-scout
---

# FujiwaraChoki/MoneyPrinter — claude-md

**Why it's worth keeping:** The ASCII architecture diagram provides indispensable context for complex workflows, and the 'Verify' section gives Claude specific ways to self-validate its changes.

**Summary:** A highly detailed technical blueprint that maps out an end-to-end media generation pipeline including data flow and module responsibilities.

**Source credibility:** Highly credible; a popular open-source project with over 13k stars.

**Recency:** Very current; utilizes modern tooling like `uv` and shows recent maintenance.

**Source:** [FujiwaraChoki/MoneyPrinter/CLAUDE.md](https://github.com/FujiwaraChoki/MoneyPrinter/blob/2a7c6bc6e8fab6e01fa740c4311d9e1e233b0262/CLAUDE.md) · 13527★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

MoneyPrinter automates YouTube Shorts creation from text topics. It uses Ollama for script generation, TikTok TTS for voiceover, Pexels for stock footage, and moviepy/ImageMagick for video composition. Output: a 9:16 vertical video (`output.mp4`).

## Commands

### Setup
```bash
cp .env.example .env        # then fill in API keys
uv sync                     # install dependencies
ollama serve                # start Ollama (separate terminal)
ollama pull llama3.1:8b     # pull default model
```

### Run (local)
```bash
uv run python Backend/main.py                              # API on :8080
uv run python Backend/worker.py                            # queue worker
python3 -m http.server 3000 --directory Frontend           # frontend on :3000
```

### Run (Docker)
```bash
docker compose up --build   # frontend :8001, backend :8080, postgres :5432
```

### Verify
```bash
uv run python -m compileall Backend          # syntax check
curl http://localhost:8080/api/models         # API smoke test
```

### Tests
No test suite exists yet. If added, use pyt
```

</details>
