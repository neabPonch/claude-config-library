---
name: OpenLAIR__dr-claw__skill
source: https://github.com/OpenLAIR/dr-claw/blob/0fab72c75368efa8f248b1d44634fe2354bee686/skills/mlops/mlflow/SKILL.md
repo: OpenLAIR/dr-claw
kind: skill
stars: 988
last_pushed: 2026-06-16T02:26:45Z
license: other
score: 9
domains: [mlops, data-science, machine-learning]
tags: [mlflow, experiment-tracking, model-registry]
curated: 2026-06-16
curated_by: config-scout
---

# OpenLAIR/dr-claw — skill

**Why it's worth keeping:** The file provides specific code idioms for different frameworks (PyTorch, Sklearn, Transformers) rather than generic descriptions. It includes critical operational details like model stage transitions and URI patterns that are essential for autonomous MLOps tasks.

**Summary:** A highly structured technical manual that enables an agent to manage the full MLflow lifecycle, including tracking, autologging, and model registry transitions.

**Source credibility:** Based on the industry-standard MLflow framework with significant community adoption (23k+ stars).

**Recency:** Current; reflects modern, framework-agnostic ML lifecycle practices.

**Source:** [OpenLAIR/dr-claw/skills/mlops/mlflow/SKILL.md](https://github.com/OpenLAIR/dr-claw/blob/0fab72c75368efa8f248b1d44634fe2354bee686/skills/mlops/mlflow/SKILL.md) · 988★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: mlflow
description: Track ML experiments, manage model registry with versioning, deploy models to production, and reproduce experiments with MLflow - framework-agnostic ML lifecycle platform
version: 1.0.0
author: Orchestra Research
license: MIT
tags: [MLOps, MLflow, Experiment Tracking, Model Registry, ML Lifecycle, Deployment, Model Versioning, PyTorch, TensorFlow, Scikit-Learn, HuggingFace]
dependencies: [mlflow, sqlalchemy, boto3]
---

# MLflow: ML Lifecycle Management Platform

## When to Use This Skill

Use MLflow when you need to:
- **Track ML experiments** with parameters, metrics, and artifacts
- **Manage model registry** with versioning and stage transitions
- **Deploy models** to various platforms (local, cloud, serving)
- **Reproduce experiments** with project configurations
- **Compare model versions** and performance metrics
- **Collaborate** on ML projects with team workflows
- **Integrate** with any ML framework (framework-agnostic)

**Users**: 20,000+ organizations | **GitHub Stars**: 23k+ | **License**: Apache 2.0

## Installation

```bash
# Install MLflow
pip install mlflow

# Install with extras
pip install mlflow[extras]  # Includes SQLAlchemy, boto3,
```

</details>
