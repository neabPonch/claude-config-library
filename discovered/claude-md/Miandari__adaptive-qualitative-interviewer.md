---
name: Miandari__adaptive-qualitative-interviewer
source: https://github.com/Miandari/adaptive-qualitative-interviewer/blob/04e237af01519a165ce0e8e2cf6ca5c426070eec/claude.md
repo: Miandari/adaptive-qualitative-interviewer
kind: claude-md
stars: 0
last_pushed: 2025-11-05T03:44:47Z
license: unknown
score: 8
domains: [agents-ai, backend-api, research]
tags: [roadmap-driven, architectural-context, constraint-aware]
curated: 2026-06-16
curated_by: config-scout
---

# Miandari/adaptive-qualitative-interviewer — claude-md

**Why it's worth keeping:** The 'Capabilities & Limitations' section is elite; it prevents the AI from attempting to modify things through YAML that require code changes. The structured Roadmap also allows an agent to understand upcoming technical debt and future goals.

**Summary:** A high-context guide that combines project architecture, a multi-phase roadmap, and strict coding standards.

**Source credibility:** Low social proof (0 stars) but demonstrates sophisticated engineering thought and research-grade structure.

**Recency:** 7 months old; highly relevant for modern LangGraph/Python development.

**Source:** [Miandari/adaptive-qualitative-interviewer/claude.md](https://github.com/Miandari/adaptive-qualitative-interviewer/blob/04e237af01519a165ce0e8e2cf6ca5c426070eec/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AI Experimenter - Development Guide

## Project Overview

**Current State:** AI Experimenter is an Experience Sampling Method (ESM) research chatbot built with LangChain/LangGraph. It conducts qualitative research interviews through conversational AI, currently supporting studies on empathy and decision-making.

**Vision:** Transform into a multi-user research framework where researchers can:
- Create and load their own experiments without modifying core code
- Customize conversation flows, data collection, and evaluation criteria
- Share experiments with other researchers
- Run isolated experiments with private prompts

## Architecture Foundation

**Core Technologies:**
- LangChain/LangGraph for conversation orchestration
- OpenAI/Anthropic LLM providers
- Multiple UI options (Streamlit primary, FastAPI for REST API)
- YAML-based experiment configuration
- Python 3.x with virtual environment (venv)

**Development Environment:**
- Uses virtual environment located in `venv/`
- Activate with: `source venv/bin/activate`
- Always use `venv/bin/python` or activate venv before running Python commands
- Dependencies managed via `requirements.txt`

**Current Structure:**
```
core/
```

</details>
