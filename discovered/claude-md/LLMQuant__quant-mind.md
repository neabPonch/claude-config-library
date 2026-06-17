---
name: LLMQuant__quant-mind
source: https://github.com/LLMQuant/quant-mind/blob/8e218884a6cec3122ba42f9fa2277d593b907361/CLAUDE.md
repo: LLMQuant/quant-mind
kind: claude-md
stars: 1381
last_pushed: 2026-06-04T05:50:23Z
license: mit
score: 9
domains: [quantitative-finance, ai-agents, backend]
tags: [architecture-driven, guardrails, high-density]
curated: 2026-06-15
curated_by: config-scout
---

# LLMQuant/quant-mind — claude-md

**Why it's worth keeping:** The 'Current Repository State' table provides high-density ground truth for the current refactor; explicit 'Architecture Principles' act as guardrails against anti-patterns; and specific 'Conventions' ensure schema/import consistency.

**Summary:** Provides deep architectural context including module status and dependency contracts to prevent the AI from resurrecting legacy code. It defines strict coding conventions and a single-source-of-truth verification workflow.

**Source credibility:** Highly credible source with 1.3k+ stars and active, recent development.

**Recency:** Very current, utilizing modern Python toolchains like uv, ruff, and basedpyright.

**Source:** [LLMQuant/quant-mind/CLAUDE.md](https://github.com/LLMQuant/quant-mind/blob/8e218884a6cec3122ba42f9fa2277d593b907361/CLAUDE.md) · 1381★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working in this repository.

## Project Overview

QuantMind is an intelligent knowledge extraction and retrieval framework for quantitative
finance. As of 2026-04, it is being **repositioned as a domain library that runs on top
of OpenAI Agents SDK**, rather than as a self-contained agent framework.

The pre-pivot agent runtime (`brain/`, `tools/`, `storage/`, `tagger/`, custom Tool ABC,
custom MultiStepAgent / Memory) was removed in PR #70. A full snapshot of the removed
code is preserved on the `archive/agent-runtime-final` branch on origin — reference it
if you need historical context, never resurrect it into master.

## Target Architecture (post-migration)

```
quantmind/
├── flows/        # e2e pipeline functions (paper_flow, news_flow, ...)
├── knowledge/    # Pydantic schemas (KnowledgeItem subclasses: Paper, News, ...)
├── preprocess/   # fetch (arxiv/http/doi/local) + format (pdf/html/markdown)
├── mind/         # cognitive layer; mind/memory/ is the MVP (filesystem-backed)
├── configs/      # centralized cfg + input types (BaseFlowCfg + per-flow types)
├── magic.py      # resolve_magic_input: na
```

</details>
