---
name: motethansen__ai_agent_assistant
source: https://github.com/motethansen/ai_agent_assistant/blob/136f630a04b74ef441eca65f2c051fdf88b7d6d9/CLAUDE.md
repo: motethansen/ai_agent_assistant
kind: claude-md
stars: 0
last_pushed: 2026-06-13T01:28:03Z
license: mit
score: 9
domains: [cli-tools, agents-ai, personal-knowledge-management]
tags: [logging-protocol, state-persistence, obsidian-integration]
curated: 2026-06-15
curated_by: config-scout
---

# motethansen/ai_agent_assistant — claude-md

**Why it's worth keeping:** The highly specific 'When/What/How' logging contract is a masterclass in maintaining state across AI sessions; the conventions section also provides excellent operational guardrails.

**Summary:** Defines a local-first AI assistant and implements a rigorous 'Vault Logging' protocol for tracking developer progress within an Obsidian vault.

**Source credibility:** Low star count indicates a personal project, but the extreme specificity suggests a sophisticated developer workflow.

**Recency:** Very current; uses future-dated context (2026) suggesting it's extremely fresh or part of an active time-shifted development loop.

**Source:** [motethansen/ai_agent_assistant/CLAUDE.md](https://github.com/motethansen/ai_agent_assistant/blob/136f630a04b74ef441eca65f2c051fdf88b7d6d9/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ai_agent_assistant — Claude Code Guide

> Read this at session start. It tells Claude what this project is, how to run it, and how to log progress into the user's Obsidian vault.

## What this project is

A **local-first personal AI assistant** that bridges Markdown notes (Obsidian + LogSeq), Apple Calendar, and task lists — all from the terminal, powered by local LLMs. Optimized for headless, low-memory operation on Apple Silicon and Linux.

- **Reads** tasks from Obsidian + LogSeq (`LATER` / `TODO` markers), Apple Reminders
- **Writes** schedule into Apple Calendar, daily plans back into Obsidian
- **Runs** offline by default; cloud LLMs are fallback only
- **Triggers** the full planning pipeline from n8n on weekdays at 08:00

**Primary LLM:** Ollama (local, headless).
**Fallback chain:** Ollama → Groq → Gemini → OpenAI → Claude.

## Key entry points

```bash
./run.sh            # main planning pipeline (reads notes, generates plan, writes back)
./install.sh        # idempotent install (creates venv, pulls Ollama models, wires cron)
python main.py      # bypass run.sh wrapper
pytest              # full test suite
```

Config lives in `.config` (env-var style — see `config.examp
```

</details>
