---
name: OpenBMB__MiniCPM__skill
source: https://github.com/OpenBMB/MiniCPM/blob/d4115377d32ad51cb2a369350b9671a478e1f015/skills/minicpm5-finetune-xtuner/SKILL.md
repo: OpenBMB/MiniCPM
kind: skill
stars: 9454
last_pushed: 2026-06-12T02:34:55Z
license: apache-2.0
score: 9
domains: [agents-ai, mlops, cli-tools]
tags: [finetune, minicpm, xtuner, lora, sft]
curated: 2026-06-15
curated_by: config-scout
---

# OpenBMB/MiniCPM — skill

**Why it's worth keeping:** It includes critical hyperparameter corrections (start_factor) and specific chat template requirements that prevent common silent training failures. The troubleshooting section addresses specific environment issues like libGL dependencies and process hanging.

**Summary:** A specialized recipe for fine-tuning MiniCPM5-1B using XTuner, providing a full Python configuration script and conversion workflow.

**Source credibility:** High; OpenBMB is a reputable source with high-star, active repositories.

**Recency:** Current; uses modern MiniCPM5 models and up-to-date training frameworks.

**Source:** [OpenBMB/MiniCPM/skills/minicpm5-finetune-xtuner/SKILL.md](https://github.com/OpenBMB/MiniCPM/blob/d4115377d32ad51cb2a369350b9671a478e1f015/skills/minicpm5-finetune-xtuner/SKILL.md) · 9454★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: minicpm5-finetune-xtuner
description: Fine-tune MiniCPM5-1B with xtuner (mmengine config-driven SFT). Use when the user mentions "xtuner", "mmengine", InternLM's training framework, or wants config-file-driven training.
---

# Fine-tune MiniCPM5-1B with xtuner

mmengine config-driven SFT. Uses Python config files (not YAML) and integrates with mmengine's runner / hook system.

## Required input

| Var | Example | Default |
| --- | --- | --- |
| `BASE_MODEL` | `openbmb/MiniCPM5-1B` | required |
| `DATA` | path to messages-format jsonl | required |
| `WORK_DIR` | `./runs/minicpm5_xtuner` | required |

## Steps

### 1. Install (once)

```bash
pip install "xtuner==0.2.0"
# Replace opencv-python with the headless variant (avoids libGL linkage)
pip install --force-reinstall opencv-python-headless
pip uninstall -y opencv-python
```

### 2. Save the config — `${WORK_DIR}/minicpm5_lora.py`

```python
import torch
from datasets import load_dataset
from mmengine.dataset import DefaultSampler
from mmengine.hooks import (CheckpointHook, DistSamplerSeedHook, IterTimerHook,
                            LoggerHook, ParamSchedulerHook)
from mmengine.optim import AmpOptimWrapper, CosineAnne
```

</details>
