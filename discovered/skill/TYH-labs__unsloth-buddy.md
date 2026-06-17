---
name: TYH-labs__unsloth-buddy
source: https://github.com/TYH-labs/unsloth-buddy/blob/e8e461ff894481090eff44be91638d6723f7e9c0/SKILL.md
repo: TYH-labs/unsloth-buddy
kind: skill
stars: 251
last_pushed: 2026-05-07T06:11:55Z
license: mit
score: 9
domains: [machine-learning, ai-agents, cli-tools]
tags: [llm-finetuning, unsloth, mlx, training-automation]
curated: 2026-06-15
curated_by: config-scout
---

# TYH-labs/unsloth-buddy — skill

**Why it's worth keeping:** Implements a sophisticated 'Roadbook' system (gaslamp, memory, progress logs) to maintain reasoning state across long-running agent sessions. It enforces strict project isolation to prevent artifact clutter during complex ML tasks.

**Summary:** An end-to-end agentic framework for LLM fine-tuning that bridges NVIDIA/Unsloth and Apple Silicon/MLX workflows. It automates environment setup, training phases, and deployment.

**Source credibility:** High; part of the specialized Gaslamp AI platform with significant community interest via GitHub stars.

**Recency:** Current; includes modern techniques like GRPO and specific Apple Silicon optimizations.

**Source:** [TYH-labs/unsloth-buddy/SKILL.md](https://github.com/TYH-labs/unsloth-buddy/blob/e8e461ff894481090eff44be91638d6723f7e9c0/SKILL.md) · 251★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: unsloth-buddy
description: This skill should be used when users want to fine-tune language models or perform reinforcement learning (SFT, DPO, GRPO, ORPO, KTO, SimPO) using the highly optimized Unsloth library. Covers environment setup, LoRA patching, VRAM optimization, vision/multimodal fine-tuning, TTS, embedding training, and GGUF/vLLM/Ollama deployment. Should be invoked for tasks involving fast, memory-efficient local or cloud GPU training, specifically when the user mentions Unsloth or when hardware limits prevent standard training.
license: Complete terms in LICENSE.txt
metadata:
  author: gaslamp
  version: "1.0.3"
  category: machine-learning
  repository: https://github.com/TYH-labs/unsloth-buddy
compatibility: "Apple Silicon (M1/M2/M3/M4): requires Python ≤ 3.12 and mlx-tune (not CUDA). Linux/WSL with NVIDIA GPU: CUDA 11.8, 12.1, or 12.4+, Python 3.10+. Windows: conda env with Python 3.12. Not compatible with standard Unsloth on Apple Silicon."
---

# Unsloth Training & Optimization

## Overview

You are the `unsloth-buddy`, a specialized AI assistant that helps machine learning practitioners train and optimize large language models (LLMs) using the Unsloth lib
```

</details>
