---
name: przeprogramowani__10x-bench
source: https://github.com/przeprogramowani/10x-bench/blob/4901b29bfd88d34a8d266ae4facd6071570e182d/CLAUDE.md
repo: przeprogramowani/10x-bench
kind: claude-md
stars: 6
last_pushed: 2026-06-09T21:21:48Z
license: mit
score: 9
domains: [web-frontend, data-processing]
tags: [astro, benchmark, data-pipeline]
curated: 2026-06-15
curated_by: config-scout
---

# przeprogramowani/10x-bench — claude-md

**Why it's worth keeping:** It defines strict formatting requirements for data inputs and establishes critical behavioral constraints (preventing the agent from reading other attempt directories) to ensure benchmark integrity.

**Summary:** A high-fidelity instruction file for managing an LLM benchmark dashboard through a specific CSV-to-JSON data pipeline.

**Source credibility:** Niche benchmarking project with recent activity.

**Recency:** Very current, referencing Astro 5.x and React 19.

**Source:** [przeprogramowani/10x-bench/CLAUDE.md](https://github.com/przeprogramowani/10x-bench/blob/4901b29bfd88d34a8d266ae4facd6071570e182d/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**10xBench** is a comprehensive benchmark comparing how different large language models handle "vibe coding"—creating a fully functional website for [Przeprogramowani.pl](https://przeprogramowani.pl) in a single attempt without iterative refinement.

Each of four models (Claude Opus 4.6, GPT-5.3-Codex, Kimi K2.5, GLM-4.7) receives the same prompt and must generate a complete website implementation. Results are systematically evaluated against defined criteria and presented in an interactive dashboard.

## Quick Start Commands

### Development & Building

```bash
# Process results CSV files and generate results.json
npm run process-results

# Start development server (Astro) with results processing
npm run dev

# Build production site
npm run build

# Development from website directory (for Astro only)
cd website && npm run dev
cd website && npm run build
```

### Evaluation

```bash
# Run the evaluation skill to assess an implementation
/10x-run-eval against <attempt-directory>

# Example:
/10x-run-eval against claude opus attempt 1
```

## Proje
```

</details>
