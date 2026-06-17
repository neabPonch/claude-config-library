---
name: maha0525__SAIVerse
source: https://github.com/maha0525/SAIVerse/blob/da48e5ea9a0f313d4789278da170a06f45f5ee45/CLAUDE.md
repo: maha0525/SAIVerse
kind: claude-md
stars: 37
last_pushed: 2026-06-12T13:13:45Z
license: agpl-3.0
score: 9
domains: [agents-ai, backend-api, cli-tools]
tags: [safety-guardrails, verification-steps, architectural-overview]
curated: 2026-06-14
curated_by: config-scout
---

# maha0525/SAIVerse — claude-md

**Why it's worth keeping:** Uses specific 'Safety Notes' to prevent destructive database operations; includes explicit 'Definition of Done' instructions like running ruff check after code modifications.

**Summary:** Provides comprehensive operational instructions including high-risk command warnings, mandatory linting steps, and architectural context for a complex multi-agent system.

**Source credibility:** Active repository with recent updates and clear, professional documentation structure.

**Recency:** Highly current; aligns perfectly with modern AI agent workflows (Claude Code/LangGraph).

**Source:** [maha0525/SAIVerse/CLAUDE.md](https://github.com/maha0525/SAIVerse/blob/da48e5ea9a0f313d4789278da170a06f45f5ee45/CLAUDE.md) · 37★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Notes for Claude Code

**Language**: Think in English, respond in Japanese. The repository owner prefers Japanese for communication.

**Local preferences**: If `CLAUDE.local.md` exists in the repository root, read it for additional context (names, personal preferences, etc.).

## Project Overview

SAIVerse is a multi-agent AI system where autonomous AI personas (agents) inhabit a virtual world composed of Cities and Buildings. The system features:

- Multiple LLM providers (OpenAI, Anthropic, Google Gemini, Ollama, llama.cpp) with automatic fallback
- Persistent long-term memory using SAIMemory (SQLite)
- Inter-city travel: personas can dispatch to other SAIVerse instances via database-mediated transactions
- SEA (Self-Evolving Agent) framework: LangGraph-based playbook system for routing conversations and autonomous behavior
- Optional Discord gateway for real-time chat integration
- Next.js frontend with REST API backend

## Development Commands

### Database Setup

**⚠️ IMPORTANT: Database Safety ⚠️**

```bash
# Initialize NEW database (⚠️ DESTROYS existing dat
```

</details>
