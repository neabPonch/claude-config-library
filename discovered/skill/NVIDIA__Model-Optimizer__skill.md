---
name: NVIDIA__Model-Optimizer__skill
source: https://github.com/NVIDIA/Model-Optimizer/blob/c4f39bd260b24d83f6f587c57ab73100d865de09/.agents/skills/evaluation/SKILL.md
repo: NVIDIA/Model-Optimizer
kind: skill
stars: 2928
last_pushed: 2026-06-15T02:19:31Z
license: apache-2.0
score: 9
domains: [ai-models, llm-inference, cli-tools, mlops]
tags: [quantization, evaluation, vllm, nemo]
curated: 2026-06-15
curated_by: config-scout
---

# NVIDIA/Model-Optimizer — skill

**Why it's worth keeping:** Employs advanced 'cross-check' logic to verify deployment flags against both web recipes and local configs; includes expert-level technical nuances for vLLM environment variables and MLflow interpolation pitfalls.

**Summary:** Guides users through the end-to-end lifecycle of evaluating quantized LLMs using the NeMo Evaluator Launcher (NEL), including config generation, deployment, and monitoring.

**Source credibility:** Highly credible: sourced from NVIDIA's active, high-star Model Optimizer repository.

**Recency:** Current, targeting modern LLM serving technologies like vLLM and SGLang.

**Source:** [NVIDIA/Model-Optimizer/.agents/skills/evaluation/SKILL.md](https://github.com/NVIDIA/Model-Optimizer/blob/c4f39bd260b24d83f6f587c57ab73100d865de09/.agents/skills/evaluation/SKILL.md) · 2928★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: evaluation
description: Evaluates accuracy of quantized or unquantized LLMs using NeMo Evaluator Launcher (NEL). Triggers on "evaluate model", "benchmark accuracy", "run MMLU", "evaluate quantized model", "run nel". Handles deployment, config generation, and evaluation execution. Not for quantizing models (use ptq), deploying/serving models (use deployment), or comparing completed baseline-vs-quantized results (use compare-results).
license: Apache-2.0
# Based on nel-assistant skill from NeMo Evaluator Launcher (commit f1fa073).
# https://github.com/NVIDIA-NeMo/Evaluator/tree/f1fa073/packages/nemo-evaluator-launcher/.claude/skills/nel-assistant
---

## NeMo Evaluator Launcher Assistant

Guide the user through creating NEL YAML configs, running evaluations, and monitoring progress.

### Workspace integration

If `MODELOPT_WORKSPACE_ROOT` is set, read `skills/common/workspace-management.md` and reuse existing workspaces (this skill is usually the final stage of PTQ → Deploy → Eval; carry any deployment-time patches into `deployment.command`).

### Workflow

```text
- [ ] Step 0: Check workspace (if MODELOPT_WORKSPACE_ROOT set)
- [ ] Step 1: Check `nel` install + existing co
```

</details>
