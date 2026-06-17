---
name: MiniMax-AI__cli__skill
source: https://github.com/MiniMax-AI/cli/blob/5f13ef51d919b069eef69fbd634c98e55310412f/skill/SKILL.md
repo: MiniMax-AI/cli
kind: skill
stars: 1923
last_pushed: 2026-06-09T12:41:42Z
license: unknown
score: 9
domains: [agents-ai, cli-tools, multimedia]
tags: [multimodal, media-generation, api-wrapper]
curated: 2026-06-14
curated_by: config-scout
---

# MiniMax-AI/cli — skill

**Why it's worth keeping:** It prioritizes non-interactive flags (--non-interactive, --quiet) and machine-readable outputs (--output json), which are essential to prevent an agent from getting stuck on progress bars or human prompts. The inclusion of async task handling (video polling/task IDs) is a high-tier technique for reliable tool use.

**Summary:** A comprehensive skill guide for using the mmx-cli to generate multi-modal content (text, image, video, speech, music). It provides structured command definitions designed specifically for agentic tool-use.

**Source credibility:** Highly credible; official documentation for a popular, highly-starred AI CLI tool.

**Recency:** Very current, following modern patterns for LLM-to-CLI interaction.

**Source:** [MiniMax-AI/cli/skill/SKILL.md](https://github.com/MiniMax-AI/cli/blob/5f13ef51d919b069eef69fbd634c98e55310412f/skill/SKILL.md) · 1923★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: mmx-cli
description: Use mmx to generate text, images, video, speech, and music via the MiniMax AI platform. Use when the user wants to create media content, chat with MiniMax models, perform web search, or manage MiniMax API resources from the terminal.
---

# MiniMax CLI — Agent Skill Guide

Use `mmx` to generate text, images, video, speech, music, and perform web search via the MiniMax AI platform.

## Prerequisites

```bash
# Install
npm install -g mmx-cli

# Auth (OAuth persists to ~/.mmx/credentials.json, API key persists to ~/.mmx/config.json)
mmx auth login --api-key sk-xxxxx

# Verify active auth source
mmx auth status

# Or pass per-call
mmx text chat --api-key sk-xxxxx --message "Hello"
```

Region is auto-detected. Override with `--region global` or `--region cn`.

---

## Agent Flags

Always use these flags in non-interactive (agent/CI) contexts:

| Flag | Purpose |
|---|---|
| `--non-interactive` | Fail fast on missing args instead of prompting |
| `--quiet` | Suppress spinners/progress; stdout is pure data |
| `--output json` | Machine-readable JSON output |
| `--async` | Return task ID immediately (video generation) |
| `--dry-run` | Preview the API reques
```

</details>
