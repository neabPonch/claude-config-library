---
name: OpenRaiser__NanoResearch__skill
source: https://github.com/OpenRaiser/NanoResearch/blob/7144364564cc2a9fe22e49fbff94eca058b5a75b/skills/vendor-ai-research/accelerate/SKILL.md
repo: OpenRaiser/NanoResearch
kind: skill
stars: 1505
last_pushed: 2026-05-26T09:16:37Z
license: mit
score: 9
domains: [machine-learning, distributed-training, pytorch]
tags: [huggingface, accelerate, deep-learning]
curated: 2026-06-15
curated_by: config-scout
---

# OpenRaiser/NanoResearch — skill

**Why it's worth keeping:** Uses explicit diff-style notation (+/-) for code transformation tasks and provides specific configuration patterns for DeepSpeed/FSDP plugins.

**Summary:** A technical reference guide for migrating standard PyTorch scripts to distributed training environments using HuggingFace Accelerate.

**Source credibility:** Highly credible source with 1.5k stars and recent maintenance activity.

**Recency:** Current, including support for modern precision formats like FP8/BF16.

**Source:** [OpenRaiser/NanoResearch/skills/vendor-ai-research/accelerate/SKILL.md](https://github.com/OpenRaiser/NanoResearch/blob/7144364564cc2a9fe22e49fbff94eca058b5a75b/skills/vendor-ai-research/accelerate/SKILL.md) · 1505★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: huggingface-accelerate
description: Simplest distributed training API. 4 lines to add distributed support to any PyTorch script. Unified API for DeepSpeed/FSDP/Megatron/DDP. Automatic device placement, mixed precision (FP16/BF16/FP8). Interactive config, single launch command. HuggingFace ecosystem standard.
version: 1.0.0
author: Orchestra Research
license: MIT
tags: [Distributed Training, HuggingFace, Accelerate, DeepSpeed, FSDP, Mixed Precision, PyTorch, DDP, Unified API, Simple]
dependencies: [accelerate, torch, transformers]
---

# HuggingFace Accelerate - Unified Distributed Training

## Quick start

Accelerate simplifies distributed training to 4 lines of code.

**Installation**:
```bash
pip install accelerate
```

**Convert PyTorch script** (4 lines):
```python
import torch
+ from accelerate import Accelerator

+ accelerator = Accelerator()

  model = torch.nn.Transformer()
  optimizer = torch.optim.Adam(model.parameters())
  dataloader = torch.utils.data.DataLoader(dataset)

+ model, optimizer, dataloader = accelerator.prepare(model, optimizer, dataloader)

  for batch in dataloader:
      optimizer.zero_grad()
      loss = model(batch)
-     loss.backward()
+
```

</details>
