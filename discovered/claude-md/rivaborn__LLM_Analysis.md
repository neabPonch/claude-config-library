---
name: rivaborn__LLM_Analysis
source: https://github.com/rivaborn/LLM_Analysis/blob/864916232c9c6773b647527c8e2a1195b18f00b2/CLAUDE.md
repo: rivaborn/LLM_Analysis
kind: claude-md
stars: 0
last_pushed: 2026-05-12T18:11:05Z
license: unknown
score: 9
domains: [cli-tools, game-development, devops-automation]
tags: [unreal-engine, pipeline-orchestration, documentation-automation]
curated: 2026-06-16
curated_by: config-scout
---

# rivaborn/LLM_Analysis — claude-md

**Why it's worth keeping:** It provides high-density context including detailed directory mappings, precise invocation patterns, and an exact orchestration pipeline. It excels at documenting technical prerequisites like LSP/clangd setup and environment variable dependencies.

**Summary:** An exhaustive operational manual for a complex automation toolkit used to document Unreal Engine architecture via the Claude CLI.

**Source credibility:** Highly specialized developer tool with significant technical depth in C++/Unreal Engine workflows.

**Recency:** Very recent; 1 month ago, highly relevant to modern LLM-driven CLI automation.

**Source:** [rivaborn/LLM_Analysis/CLAUDE.md](https://github.com/rivaborn/LLM_Analysis/blob/864916232c9c6773b647527c8e2a1195b18f00b2/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md -- Project Context

## Project Overview

Architecture documentation toolkit for Unreal Engine source code. Generates per-file and subsystem-level architecture docs using the **Claude CLI** (`claude -p`), with optional LSP-powered semantic analysis via clangd.

**Target Codebase:** Unreal Engine 5.7.3 (Epic Games), `C:\Coding\Epic_Games\UnrealEngine` (fork of EpicGames/UnrealEngine, branch `release`).
**LLM Backend:** Anthropic Claude via the local `claude` CLI. Default model `haiku`, with tiered auto-upgrade to `sonnet` for complex files.
**Sister Toolkit:** `C:\Coding\LocalLLM_Analysis` is the Ollama variant of this same toolkit. The two share an identical `Common/llm_common.ps1` shim and `Common/file_helpers.ps1`; they differ in `Common/llm_core.ps1` (lean here, full Ollama API client there) and `Common/.env` (Claude CLI keys here, Ollama keys there).
**System:** Windows 11, 32 GB RAM.

## Directory Layout

The toolkit is split into a shared module folder (`Common/`) and a pipeline folder (`Analysis/`). Drop the whole `LLM_Analysis/` directory anywhere; scripts find each other via sibling-relative paths.

```
<toolkit root>/                     (e.g. C:\Coding\LLM_Ana
```

</details>
