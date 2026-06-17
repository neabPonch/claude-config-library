---
name: pinchbench__skill
source: https://github.com/pinchbench/skill/blob/819384ae830492365b8363fc26bc2602e73f216d/SKILL.md
repo: pinchbench/skill
kind: skill
stars: 1230
last_pushed: 2026-06-02T21:35:43Z
license: mit
score: 8
domains: [agents-ai, cli-tools, evaluation]
tags: [benchmarking, llm-evals]
curated: 2026-06-14
curated_by: config-scout
---

# pinchbench/skill — skill

**Why it's worth keeping:** The task definition structure—combining YAML frontmatter with automated Python grading functions—is a professional-grade template for building reliable agent evaluations.

**Summary:** A benchmarking suite designed to evaluate LLM agent performance across diverse, multi-step real-world tasks.

**Source credibility:** High; 1200+ stars and active maintenance by Kilo.ai suggest a highly useful, community-vetted tool.

**Recency:** Current; utilizes modern tooling like `uv` and reflects contemporary LLM model nomenclature.

**Source:** [pinchbench/skill/SKILL.md](https://github.com/pinchbench/skill/blob/819384ae830492365b8363fc26bc2602e73f216d/SKILL.md) · 1230★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pinchbench
description: Run PinchBench benchmarks to evaluate OpenClaw agent performance across real-world tasks. Use when testing model capabilities, comparing models, submitting benchmark results to the leaderboard, or checking how well your OpenClaw setup handles calendar, email, research, coding, and multi-step workflows.
metadata:
  author: pinchbench
  version: "2.0.0-rc1"
  homepage: https://pinchbench.com
  repository: https://github.com/pinchbench/skill
---

# PinchBench Benchmark Skill

PinchBench measures how well LLM models perform as the brain of an OpenClaw agent. Results are collected on a public leaderboard at [pinchbench.com](https://pinchbench.com).

## Prerequisites

- Python 3.10+
- [uv](https://docs.astral.sh/uv/) package manager
- OpenClaw instance (this agent)

## Quick Start

```bash
cd <skill_directory>

# Run benchmark with a specific model
uv run benchmark.py --model anthropic/claude-sonnet-4

# Run only automated tasks (faster)
uv run benchmark.py --model anthropic/claude-sonnet-4 --suite automated-only

# Run specific tasks
uv run benchmark.py --model anthropic/claude-sonnet-4 --suite task_calendar,task_stock

# Skip uploading results
uv run b
```

</details>
