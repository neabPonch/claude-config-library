---
name: mihnin__Code_analiz
source: https://github.com/mihnin/Code_analiz/blob/b7f79429c61c10e43b6a871bb1b0480c3f562f4f/claude.md
repo: mihnin/Code_analiz
kind: claude-md
stars: 0
last_pushed: 2026-05-18T06:02:12Z
license: mit
score: 9
domains: [web-frontend, ai-agents, security]
tags: [spa, llm-streaming, architecture-deep-dive, security]
curated: 2026-06-14
curated_by: config-scout
---

# mihnin/Code_analiz — claude-md

**Why it's worth keeping:** It excels at documenting nuanced edge cases like TTFB vs. idle timeouts and DoS guards; it also provides specific verification commands for syntax validation and behavioral tests.

**Summary:** A highly detailed technical blueprint for a zero-dependency SPA that explains complex LLM streaming protocols, security boundaries, and state management logic.

**Source credibility:** Low social proof (0 stars), but the extreme depth of technical detail suggests a high level of engineering rigor.

**Recency:** Very current, referencing modern reasoning models and advanced web-standard patterns.

**Source:** [mihnin/Code_analiz/claude.md](https://github.com/mihnin/Code_analiz/blob/b7f79429c61c10e43b6a871bb1b0480c3f562f4f/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**AI сканер** — Role-Based AI Code Assistant SPA for enterprise analysis of source code, functional specifications (ФС), and technical requirements (ТЗ). Supports ABAP, 1C, Python, JavaScript. Three roles: InfoSec, Consultant, Developer. Connects to cloud API (DeepSeek) or local models (LM Studio, Ollama, Xinference) via OpenAI-compatible protocol.

## Running

No build tools, no npm, no bundlers. Open `index.html` directly in a browser. Fully autonomous — zero external dependencies.

**Deployment files** (air-gapped/КСПД): `index.html`, `styles.css`, `app.js`, `logo.png` — 4 files in one folder. `grep` confirms no other assets referenced anywhere.

**Syntax check**: `node -c app.js` (no runtime needed, just syntax validation). Run this after any non-trivial edit.

**Build deploy archive** (for handing to a colleague / server admin): `AI-scanner.zip` contains only `index.html`, `styles.css`, `app.js`, and `logo.png` at the archive root. The archive **is committed to the repo** for direct GitHub-download distribution — rebuild it after any change
```

</details>
