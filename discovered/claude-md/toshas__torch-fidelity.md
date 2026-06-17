---
name: toshas__torch-fidelity
source: https://github.com/toshas/torch-fidelity/blob/5e211a950a7b45206bd4976813ffd6aed6cf4ccc/CLAUDE.md
repo: toshas/torch-fidelity
kind: claude-md
stars: 1190
last_pushed: 2026-05-11T17:16:03Z
license: other
score: 9
domains: [machine-learning, computer-vision, python-library]
tags: [pytorch, metrics, testing-heavy, scientific-computing]
curated: 2026-06-15
curated_by: config-scout
---

# toshas/torch-fidelity — claude-md

**Why it's worth keeping:** The granular breakdown of multiple test 'flavors' (including hardware/GPU requirements) is exceptional for preventing execution errors. The file tree also maps responsibilities to modules rather than just listing filenames, providing vital semantic context.

**Summary:** Provides deep context on a complex PyTorch environment by detailing module purposes and specific testing workflows. It effectively bridges the gap between high-level architecture and low-level execution requirements.

**Source credibility:** High-quality scientific library with significant community adoption (1k+ stars).

**Recency:** Current; accounts for modern PyTorch/CUDA environments and recent versioning.

**Source:** [toshas/torch-fidelity/CLAUDE.md](https://github.com/toshas/torch-fidelity/blob/5e211a950a7b45206bd4976813ffd6aed6cf4ccc/CLAUDE.md) · 1190★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

**torch-fidelity** is a PyTorch library providing epsilon-exact implementations of generative model evaluation metrics: Inception Score (ISC), Frechet Inception Distance (FID), Kernel Inception Distance (KID), Precision/Recall/F-score (PRC), Perceptual Path Length (PPL), and Monge Inception Distance (MIND). The library prioritizes numerical fidelity with reference TensorFlow implementations.

Current version: **0.4.0** (`torch_fidelity/version.py`)

## Repository Structure

```
torch_fidelity/           # Main package (~4100 lines, 29 modules)
  metrics.py              # Orchestration: calculate_metrics() entry point
  metric_isc.py           # Inception Score
  metric_fid.py           # Frechet Inception Distance
  metric_kid.py           # Kernel Inception Distance (poly/rbf kernels)
  metric_prc.py           # Precision, Recall, F-score
  metric_ppl.py           # Perceptual Path Length
  metric_mind.py          # Monge Inception Distance (sliced 2-Wasserstein)
  feature_extractor_base.py         # Abstract base for feature extractors
  feature_extractor_inceptionv3.py  # InceptionV3 (TF-compatible weights)
  feature_extractor_clip.py         #
```

</details>
