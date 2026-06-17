---
name: local-inference-lab__rtx6kpro__kld-eval-skill
source: https://github.com/local-inference-lab/rtx6kpro/blob/f6b28a3151e0e33ac17ad2ad515c50414c06a737/scripts/kld-eval-skill.md
repo: local-inference-lab/rtx6kpro
kind: skill
stars: 425
last_pushed: 2026-06-15T08:08:37Z
license: unknown
score: 9
domains: [ai-infrastructure, llm-evaluation, devops]
tags: [kld, quantization, sglang, benchmarking]
curated: 2026-06-15
curated_by: config-scout
---

# local-inference-lab/rtx6kpro — skill

**Why it's worth keeping:** Includes expert-level procedural safeguards like specific PID management to avoid killing bash sessions, patch verification steps, and quantitative benchmarks for result validation.

**Summary:** Automates multi-phase KL divergence (KLD) evaluation to compare quantized model quality against FP8 reference distributions using SGLang and Docker.

**Source credibility:** High-signal specialized repo focusing on high-end GPU inference optimizations.

**Recency:** Current; utilizes modern Qwen3.5 architectures and latest SGLang patterns.

**Source:** [local-inference-lab/rtx6kpro/scripts/kld-eval-skill.md](https://github.com/local-inference-lab/rtx6kpro/blob/f6b28a3151e0e33ac17ad2ad515c50414c06a737/scripts/kld-eval-skill.md) · 425★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: kld-eval
description: Run KLD (KL divergence) evaluation for quantized models. Measures quality loss vs FP8 reference using full vocabulary logit distributions on WikiText-2. Use when the user asks to measure KLD, compare model quality, or evaluate quantization.
user-invocable: true
allowed-tools: Bash, Read, Write, Grep, Glob, Agent
argument-hint: [action] [model-or-backend]
---

# KLD Evaluation Skill

Measures KL divergence between a quantized model and an FP8 reference using full vocabulary logit distributions captured during prefill on WikiText-2.

## Arguments

`$ARGUMENTS` can be:
- `ref` — create FP8 reference logits
- `test <model-or-backend>` — capture test model logits
- `compute` — compute KLD from existing logits
- `full` — run full pipeline (ref + test + compute)
- empty — show status of existing logit captures

## Docker Image

Use `voipmonitor/sglang:test-cu132` which has the KLD patch baked in. If using a different container, apply the patch first:

```bash
python /workspace/sglang-kld-logit-capture.py  # if baked into image
# OR copy and run from host:
docker cp patches/sglang-kld-logit-capture.py <container>:/tmp/
docker exec <container> python /tmp/sgl
```

</details>
