---
name: NVIDIA__TensorRT-LLM__skill
source: https://github.com/NVIDIA/TensorRT-LLM/blob/4f466535a4173023a1377fe172362d2259204705/.claude/skills/perf-torch-cuda-graphs/SKILL.md
repo: NVIDIA/TensorRT-LLM
kind: skill
stars: 13870
last_pushed: 2026-06-14T03:17:02Z
license: other
score: 9
domains: [mlops, performance-tuning]
tags: [cuda, pytorch, optimization]
curated: 2026-06-15
curated_by: config-scout
---

# NVIDIA/TensorRT-LLM — skill

**Why it's worth keeping:** The inclusion of a 'Decision Flowchart' and performance 'Symptoms' allows an agent to act as a performance engineer. It provides actionable Nsight Systems commands for empirical verification.

**Summary:** A highly technical guide for optimizing PyTorch workloads using CUDA Graphs across various levels of abstraction (standard PyTorch to Megatron-LM). It includes specific profiling commands and decision-making logic.

**Source credibility:** Extremely high; authored by NVIDIA for their industry-standard TensorRT-LLM repository.

**Recency:** Highly current, focusing on modern PyTorch and Megatron-LM optimization workflows.

**Source:** [NVIDIA/TensorRT-LLM/.claude/skills/perf-torch-cuda-graphs/SKILL.md](https://github.com/NVIDIA/TensorRT-LLM/blob/4f466535a4173023a1377fe172362d2259204705/.claude/skills/perf-torch-cuda-graphs/SKILL.md) · 13870★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: perf-torch-cuda-graphs
description: >-
  Apply CUDA Graphs to PyTorch workloads — API selection (torch.compile, PyTorch
  make_graphed_callables, TE make_graphed_callables, MCore CudaGraphManager,
  FullCudaGraphWrapper, manual torch.cuda.graph), code compatibility, capture
  workflows, dynamic pattern handling, and troubleshooting.
  Triggers: CUDA graph, torch.cuda.graph, make_graphed_callables, reduce-overhead,
  graph capture, graph replay, kernel launch overhead, CudaGraphManager,
  FullCudaGraphWrapper, full-iteration graph, stream capture.
tags:
  - cuda-graph
  - optimization
  - pytorch
license: Apache-2.0
metadata:
  author: NVIDIA Corporation
---

# CUDA Graphs for PyTorch

CUDA Graphs capture a sequence of GPU operations once and replay them with
minimal CPU overhead. This skill guides applying CUDA Graphs to PyTorch
training and inference workloads using native PyTorch APIs, Transformer
Engine, and Megatron-LM.

## When to Use

Reach for this skill when you encounter:

- **Triggers**: User wants to optimize with CUDA Graphs, reduce kernel launch
  overhead, or speed up training/inference loops
- **Symptoms**: Low GPU utilization (<80%), many small kernel laun
```

</details>
