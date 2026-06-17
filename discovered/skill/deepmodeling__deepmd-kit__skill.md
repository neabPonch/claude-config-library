---
name: deepmodeling__deepmd-kit__skill
source: https://github.com/deepmodeling/deepmd-kit/blob/84f854134c5bf071f86f12ad70ac30226aa3afa6/skills/deepmd-python-inference/SKILL.md
repo: deepmodeling/deepmd-kit
kind: skill
stars: 1965
last_pushed: 2026-06-15T23:55:21Z
license: lgpl-3.0
score: 9
domains: [scientific-computing, machine-learning, cli-tools]
tags: [deepmd, inference, molecular-dynamics]
curated: 2026-06-16
curated_by: config-scout
---

# deepmodeling/deepmd-kit — skill

**Why it's worth keeping:** The 'Agent Responsibilities' section provides excellent decision logic for task planning, while the detailed specification of NumPy array shapes prevents common shape-mismatch errors during code generation.

**Summary:** A highly specialized skill file for performing inference and evaluation using the DeePMD-kit deep learning package. It covers Python API usage (DeepPot), CLI tools, and handling various model formats.

**Source credibility:** High; based on a high-star, actively maintained scientific repository.

**Recency:** Current; provides modern API patterns and compatibility details.

**Source:** [deepmodeling/deepmd-kit/skills/deepmd-python-inference/SKILL.md](https://github.com/deepmodeling/deepmd-kit/blob/84f854134c5bf071f86f12ad70ac30226aa3afa6/skills/deepmd-python-inference/SKILL.md) · 1965★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: deepmd-python-inference
description: Run Python inference with DeePMD-kit models using the DeepPot API. Use when the user wants to load a trained/frozen DeePMD model (.pth or .pb) or a built-in pretrained model (e.g., DPA-3.2-5M) in Python, predict energy/force/virial for atomic configurations, evaluate descriptors, or calculate model deviation between multiple models. Also covers using `dp test` CLI for batch evaluation against labeled data.
compatibility: Requires deepmd-kit Python package installed. PyTorch backend for .pth models, TensorFlow for .pb models.
license: LGPL-3.0-or-later
metadata:
  author: iProzd
  version: '1.0'
  repository: https://github.com/deepmodeling/deepmd-kit
---

# DeePMD-kit Python Inference

Load a trained DeePMD-kit model in Python and predict energy, forces, and virial for atomic configurations. Also covers CLI-based testing with `dp test`.

## Quick Start

```python
from deepmd.infer import DeepPot
import numpy as np

dp = DeepPot("model.pth")
coord = np.array([[1, 0, 0], [0, 0, 1.5], [1, 0, 3]]).reshape([1, -1])
cell = np.diag(10 * np.ones(3)).reshape([1, -1])
atype = [1, 0, 1]
e, f, v = dp.eval(coord, cell, atype)
```

## Agent Responsi
```

</details>
