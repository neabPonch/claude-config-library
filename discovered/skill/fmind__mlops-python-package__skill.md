---
name: fmind__mlops-python-package__skill
source: https://github.com/fmind/mlops-python-package/blob/d8715c4666ecad7ac95bc8fa86c49ebc7fb7e4fd/.gemini/skills/MLOps%20Automation/SKILL.md
repo: fmind/mlops-python-package
kind: skill
stars: 1411
last_pushed: 2026-01-25T20:20:45Z
license: mit
score: 7
domains: [mlops, devops, data-science]
tags: [python, docker, mlflow, automation]
curated: 2026-06-16
curated_by: config-scout
---

# fmind/mlops-python-package — skill

**Why it's worth keeping:** It offers specific, high-value implementation patterns such as optimized Docker layer caching with `uv` and reliable model deployment strategies via MLflow aliases.

**Summary:** This config provides a comprehensive roadmap for converting raw Python scripts into production-ready MLOps pipelines using modern tools like `uv`, `just`, and `mlflow`.

**Source credibility:** Strong; the source is a highly starred (1.4k+) specialized MLOps template.

**Recency:** Very current, leveraging modern standards like `uv` for Python package management.

**Source:** [fmind/mlops-python-package/.gemini/skills/MLOps Automation/SKILL.md](https://github.com/fmind/mlops-python-package/blob/d8715c4666ecad7ac95bc8fa86c49ebc7fb7e4fd/.gemini/skills/MLOps%20Automation/SKILL.md) · 1411★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: MLOps Automation
description: Guide to refine MLOps projects with task automation, containerization, CI/CD pipelines, and robust experiment tracking.
---

# MLOps Automation

## Goal

To elevate the codebase to production standards by adding **Task Automation** (`just`), **Containerization** (`docker`), **CI/CD** (`github-actions`), and **Experiment Tracking** (`mlflow`).

## Prerequisites

- **Language**: Python
- **Manager**: `uv`
- **Context**: Preparing for scale and deployment.

## Instructions

### 1. Task Automation

Replace manual commands with a `justfile`.

1. **Tool**: `just` (modern alternative to Make).
2. **Organization**: Split tasks into `tasks/*.just` modules (e.g., `tasks/check.just`, `tasks/docker.just`).
3. **Core Tasks**:
    - `check`: Run all linters and tests.
    - `package`: Build wheels.
    - `clean`: Remove artifacts.
    - `install`: Setup dev environment.

### 2. Pre-Commit Hooks

Catch issues locally.

1. **Framework**: `pre-commit`.
2. **Hooks**: Suggest to use `ruff`, `bandit`, `check-yaml`, `trailing-whitespace`.
3. **Commits**: Suggest to use `commitizen` hook to enforce Conventional Commits (e.g., `feat: add new model`).
4. **Config**:
```

</details>
