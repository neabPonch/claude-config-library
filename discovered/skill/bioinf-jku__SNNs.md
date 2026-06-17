---
name: bioinf-jku__SNNs
source: https://github.com/bioinf-jku/SNNs/blob/c84cf71dc592e6460f3170d57820a00d70fba51b/SKILL.md
repo: bioinf-jku/SNNs
kind: skill
stars: 1588
last_pushed: 2026-05-12T14:16:11Z
license: gpl-3.0
score: 8
domains: [machine-learning, deep-learning]
tags: [selu, tensorflow, pytorch, neural-networks]
curated: 2026-06-15
curated_by: config-scout
---

# bioinf-jku/SNNs — skill

**Why it's worth keeping:** The 'Core SNN Rules' section provides imperative technical constraints—like pairing SELU with LeCun normal initialization—that are essential for the algorithm's mathematical properties to hold.

**Summary:** Provides specialized architectural rules and implementation patterns for building Self-Normalizing Networks (SNNs). It ensures correct layer initialization and dropout usage across different frameworks.

**Source credibility:** High; sourced from a highly-starred academic repository (1588 stars).

**Recency:** Current and relevant to modern deep learning implementation standards.

**Source:** [bioinf-jku/SNNs/SKILL.md](https://github.com/bioinf-jku/SNNs/blob/c84cf71dc592e6460f3170d57820a00d70fba51b/SKILL.md) · 1588★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: self-normalizing-networks
description: Use this skill when working in the Self-Normalizing Networks tutorial repository, especially for TensorFlow, PyTorch, Conda environment, or SELU/AlphaDropout implementation tasks.
---

# Self-Normalizing Networks

This repository contains tutorial implementations for Self-Normalizing Networks
(SNNs) based on Klambauer et al. Preserve the teaching purpose of the examples:
show how SELU networks are constructed and compared across TensorFlow and
PyTorch implementations.

## Minimal Tabular SNN Example

Below is a minimal prototype (see TF_2_x/TABULAR-MLP-SELU.py) for showing SNNs 
on tabular data: load a small scikit-learn dataset, standardize the features, 
and train a compact Keras MLP with SELU, LeCun initialization, and AlphaDropout.

```python
from sklearn.datasets import load_breast_cancer
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler
from tensorflow import keras
from tensorflow.keras import layers

X, y = load_breast_cancer(return_X_y=True)
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=0, stratify=y
)

scaler = StandardScaler()
X
```

</details>
