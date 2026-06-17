---
name: ruvnet__RuView
source: https://github.com/ruvnet/RuView/blob/d639c747df4054dd50dde7de715a804a56a039bb/CLAUDE.md
repo: ruvnet/RuView
kind: claude-md
stars: 74238
last_pushed: 2026-06-17T01:08:12Z
license: mit
score: 9
domains: [rust, embedded-systems, signal-processing, computer-vision]
tags: [monorepo-mapping, adr-integration, structured-metadata]
curated: 2026-06-17
curated_by: config-scout
---

# ruvnet/RuView — claude-md

**Why it's worth keeping:** The use of tables for crate/module lookup is highly efficient for LLM context; linking specific code paths to Architecture Decision Records (ADRs) provides the 'why' behind complex logic.

**Summary:** Provides a high-density, structured map of a multi-crate Rust workspace and its specialized signal processing modules. It bridges low-level implementation details with high-level architecture through extensive ADR references.

**Source credibility:** Extremely high, originating from a large-scale, high-star specialized hardware/software project.

**Recency:** Highly current, featuring active development and recent architectural proposals.

**Source:** [ruvnet/RuView/CLAUDE.md](https://github.com/ruvnet/RuView/blob/d639c747df4054dd50dde7de715a804a56a039bb/CLAUDE.md) · 74238★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Configuration — WiFi-DensePose + Claude Flow V3

## Project: wifi-densepose

WiFi-based human pose estimation using Channel State Information (CSI).
Dual codebase: Python v1 (`v1/`) and Rust port (`v2/`).
### Key Rust Crates
| Crate | Description |
|-------|-------------|
| `wifi-densepose-core` | Core types, traits, error types, CSI frame primitives |
| `wifi-densepose-signal` | SOTA signal processing + RuvSense multistatic sensing (16 modules) |
| `wifi-densepose-nn` | Neural network inference (ONNX, PyTorch, Candle backends) |
| `wifi-densepose-train` | Training pipeline with ruvector integration + ruview_metrics; MAE pretraining recipe (`mae.rs`, ADR-152 §2.3) + WiFlow-STD port (`wiflow_std/`, tch-gated) |
| `wifi-densepose-mat` | Mass Casualty Assessment Tool — disaster survivor detection |
| `wifi-densepose-hardware` | ESP32 aggregator, TDM protocol, channel hopping firmware; `ieee80211bf/` 802.11bf forward-compat protocol model (ADR-153) |
| `wifi-densepose-ruvector` | RuVector v2.0.4 integration + cross-viewpoint fusion (5 modules) |
| `wifi-densepose-wasm` | WebAssembly bindings for browser deployment |
| `wifi-densepose-cli` | CLI tool (`wifi-densepose` bina
```

</details>
