---
name: mutable-state-inc__siliconswarm-at-ensue-plugin
source: https://github.com/mutable-state-inc/siliconswarm-at-ensue-plugin/blob/ec54af9501d4bfd0cf3a4b162e59022dee2118cb/CLAUDE.md
repo: mutable-state-inc/siliconswarm-at-ensue-plugin
kind: claude-md
stars: 2
last_pushed: 2026-03-27T18:28:58Z
license: unknown
score: 8
domains: [systems-programming, ai-hardware, rust]
tags: [architecture-mapping, api-reference]
curated: 2026-06-16
curated_by: config-scout
---

# mutable-state-inc/siliconswarm-at-ensue-plugin — claude-md

**Why it's worth keeping:** The 'Key files' table and the exhaustive list of ANE operations are perfect patterns for teaching agents about low-level/specialized APIs to prevent hallucination.

**Summary:** Provides high-density technical context through an architectural map and a comprehensive list of hardware-specific primitives.

**Source credibility:** Specialized research project focused on Apple Silicon internals.

**Recency:** Highly current, referencing M4 hardware.

**Source:** [mutable-state-inc/siliconswarm-at-ensue-plugin/CLAUDE.md](https://github.com/mutable-state-inc/siliconswarm-at-ensue-plugin/blob/ec54af9501d4bfd0cf3a4b162e59022dee2118cb/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# autoresearch-ane-at-home

Rust bindings for Apple Neural Engine via reverse-engineered private API (`_ANEInMemoryModel`). Benchmarking direct ANE access vs Apple's CoreML on the same hardware.

## Quick start

```bash
claude --plugin-dir /path/to/autoresearch-ane-at-home-plugin
```

Then type `/autoresearch` to start the autonomous optimization loop. The agent handles setup, benchmarking, and optimization automatically.

To run manually:

```bash
make setup   # install Rust + Python deps, compile, download models, detect chip+RAM
make bench   # run ANE private API benchmark
```

## Benchmark

**Model:** DistilBERT (distilbert-base-uncased-finetuned-sst-2-english), sequence length 128, batch size 1.

**Metric:** median end-to-end inference latency (embedding + transformer layers + classifier). Lower is better.

**CoreML baseline** uses Apple's open-sourced [ml-ane-transformers](https://github.com/apple/ml-ane-transformers) model (`apple/ane-distilbert-base-uncased-finetuned-sst-2-english`). This is not a vanilla DistilBERT — Apple restructured the architecture for ANE: channel-last layouts, linear layers replaced with 1x1 convolutions, large matmuls split into ANE-friendly sizes.
```

</details>
