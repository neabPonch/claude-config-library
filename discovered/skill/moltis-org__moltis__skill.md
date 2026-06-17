---
name: moltis-org__moltis__skill
source: https://github.com/moltis-org/moltis/blob/48c9a41926d095173654030a4a87baf236792b19/crates/skills/src/assets/mlops/inference/llama-cpp/SKILL.md
repo: moltis-org/moltis
kind: skill
stars: 2740
last_pushed: 2026-06-14T02:30:59Z
license: mit
score: 9
domains: [agents-ai, cli-tools, machine-learning, deployment]
tags: [llama-cpp, gguf, quantization, local-llm, inference]
curated: 2026-06-15
curated_by: config-scout
---

# moltis-org/moltis — skill

**Why it's worth keeping:** Provides highly specific expert knowledge on imatrix (importance matrix) calibration and detailed quantization tables that are essential for production-grade local deployments. Includes actionable hardware-specific build flags for Apple Silicon and NVIDIA/AMD.

**Summary:** A comprehensive technical guide for local LLM inference using llama.cpp and the GGUF format. It covers installation, hardware acceleration, Python bindings, and high-quality quantization workflows.

**Source credibility:** High; sourced from high-star repositories like moltis and linked to the well-regarded hermes-agent ecosystem.

**Recency:** Very current, including support details for Llama 3.1 and recent Apple Silicon architecture.

**Source:** [moltis-org/moltis/crates/skills/src/assets/mlops/inference/llama-cpp/SKILL.md](https://github.com/moltis-org/moltis/blob/48c9a41926d095173654030a4a87baf236792b19/crates/skills/src/assets/mlops/inference/llama-cpp/SKILL.md) · 2740★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: llama-cpp
description: Run LLM inference with llama.cpp on CPU, Apple Silicon, AMD/Intel GPUs, or NVIDIA — plus GGUF model conversion and quantization (2–8 bit with K-quants and imatrix). Covers CLI, Python bindings, OpenAI-compatible server, and Ollama/LM Studio integration. Use for edge deployment, M1/M2/M3/M4 Macs, CUDA-less environments, or flexible local quantization.
origin:
  source: hermes-agent
  url: https://github.com/nousresearch/hermes-agent
  version: 9f22977f
---

# llama.cpp + GGUF

Pure C/C++ LLM inference with minimal dependencies, plus the GGUF (GPT-Generated Unified Format) standard used for quantized weights. One toolchain covers conversion, quantization, and serving.

## When to use

**Use llama.cpp + GGUF when:**
- Running on CPU-only machines or Apple Silicon (M1/M2/M3/M4) with Metal acceleration
- Using AMD (ROCm) or Intel GPUs where CUDA isn't available
- Edge deployment (Raspberry Pi, embedded systems, consumer laptops)
- Need flexible quantization (2–8 bit with K-quants)
- Want local AI tools (LM Studio, Ollama, text-generation-webui, koboldcpp)
- Want a single binary deploy without Docker/Python

**Key advantages:**
- Universal hardware: CPU,
```

</details>
