---
name: lorenzo1285__mlops-portfolio
source: https://github.com/lorenzo1285/mlops-portfolio/blob/34bbd433adba2bbd058ab2cdc901fd5c92a3682a/CLAUDE.md
repo: lorenzo1285/mlops-portfolio
kind: claude-md
stars: 0
last_pushed: 2026-05-14T20:17:10Z
license: unknown
score: 9
domains: [mlops, data-science, devops]
tags: [pipeline, dvc, mlflow, kubeflow, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# lorenzo1285/mlops-portfolio — claude-md

**Why it's worth keeping:** It establishes strict architectural 'constitutions' (e.g., separating business logic from I/O) and provides granular implementation details of the ML pipeline stages.

**Summary:** A high-density technical manual for a complex MLOps pipeline using DVC, MLflow, and Kubeflow.

**Source credibility:** Low star count due to being a personal portfolio, but the technical depth suggests high-quality manual curation.

**Recency:** 

**Source:** [lorenzo1285/mlops-portfolio/CLAUDE.md](https://github.com/lorenzo1285/mlops-portfolio/blob/34bbd433adba2bbd058ab2cdc901fd5c92a3682a/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
﻿# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**MLOps Learning Portfolio — Crash Severity Use Case**

A 10-stage ML pipeline on the CGR crash dataset (Grand Rapids, 74,309 rows, 142 cols)
demonstrating the full MLOps toolchain: DVC, Great Expectations, MLflow, Kubeflow
Pipelines, and Katib (HPO).

Pipeline: `validate → ingest → featurize → [train_vae ‖ augment] → encode → [train_ml ‖ train_dl ‖ train_gmm] → evaluate → tune → register`

- `train_vae` and `augment` run in parallel (both depend only on featurize outputs)
- `train_ml`, `train_dl`, and `train_gmm` run in parallel (all depend on encode outputs)
- All other stages are sequential to avoid RAM contention on a single machine
- All stages call `dvc repro <stage>` — both locally and as KFP components
- **Class-based architecture**: each stage has a business-logic class and a thin `run.py` entry point that handles config, I/O, and MLflow logging only. Classes accept all parameters via constructor — no env var reads or file I/O inside them (constitution XIV)
- All stage scripts read config via `src/config.py` typed dataclasses — no raw y
```

</details>
