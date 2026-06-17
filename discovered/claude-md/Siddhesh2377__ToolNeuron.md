---
name: Siddhesh2377__ToolNeuron
source: https://github.com/Siddhesh2377/ToolNeuron/blob/5df5f8eaa1f199d6920ebe5cdd30cdf0db37f290/CLAUDE.md
repo: Siddhesh2377/ToolNeuron
kind: claude-md
stars: 418
last_pushed: 2026-05-18T03:57:32Z
license: mit
score: 10
domains: [android, security, ai-on-device]
tags: [architecture-driven, security-first, strict-constraints]
curated: 2026-06-15
curated_by: config-scout
---

# Siddhesh2377/ToolNeuron — claude-md

**Why it's worth keeping:** The 'Hard rules' section uses enforceable constraints (e.g., specific directory structures, comment bans, and storage requirements) to minimize AI drift. It also includes detailed technical descriptions of low-level logic like the Keystore DEK flow, which is essential for maintaining security-critical code.

**Summary:** A highly prescriptive guide for a high-security Android project that enforces strict architectural invariants and cryptographic protocols. It prevents regression by explicitly defining module boundaries and critical data flows.

**Source credibility:** A specialized, high-complexity Android/AI project with recent activity and clear architectural depth.

**Recency:** Extremely current, incorporating modern cryptographic standards and specific build-time edge cases.

**Source:** [Siddhesh2377/ToolNeuron/CLAUDE.md](https://github.com/Siddhesh2377/ToolNeuron/blob/5df5f8eaa1f199d6920ebe5cdd30cdf0db37f290/CLAUDE.md) · 418★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ToolNeuron — Repo Guide

Project memory for this repo. **When you change anything that affects future work — architecture, security behavior, new features, deprecated paths, public APIs, native JNI contracts, new scope — update this file as part of the same change.** A future session reads this to reconstruct intent; if it drifts, work breaks.

---

## Project scope

Privacy-first, offline-only on-device AI assistant. No Google Play services, no network telemetry, no analytics. In-scope pillars: on-device LLM chat, RAG over user documents, vision-language models (VLM), voice (TTS+STT), Remote Server with bundled web UI, HF Explorer, **on-device image generation / img2img / inpaint / 4× upscale via the `:ai_sd` AAR (re-pivoted in 2026-05-08)**, **first-party plugin system with ONNX inference + capability-gated APIs (re-pivoted in 2026-05-11)**. Out of scope: tool calling, Termux integration. (Image generation was originally cut on 2026-04-20 and re-added on 2026-05-08. Plugin marketplace was also originally cut on 2026-04-20 and re-added on 2026-05-11 as a first-party plugin runtime — DexClassLoader, Plugin contract with @Composable Content(), capability-gated OnnxApi/HxsApi/Netwo
```

</details>
