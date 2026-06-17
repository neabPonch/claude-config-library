---
name: NVIDIA__Isaac-GR00T
source: https://github.com/NVIDIA/Isaac-GR00T/blob/65cc4a192e6d084650d97747308b6a8deb790722/CLAUDE.md
repo: NVIDIA/Isaac-GR00T
kind: claude-md
stars: 7337
last_pushed: 2026-06-12T01:01:38Z
license: apache-2.0
score: 9
domains: [robotics, ai-models, computer-vision, embedded-systems]
tags: [robotics, vla, nvidia, deployment, high-performance-computing]
curated: 2026-06-15
curated_by: config-scout
---

# NVIDIA/Isaac-GR00T — claude-md

**Why it's worth keeping:** Includes 'Key entry points' that map high-level tasks to specific CLI commands; offers critical platform-specific environment details (CUDA versions/hardware paths) essential for robotics development.

**Summary:** Provides highly actionable command-line patterns for training, inference, and deployment across diverse hardware targets.

**Source credibility:** Extremely high; NVIDIA is an industry leader and the repo shows active maintenance.

**Recency:** Very current; utilizes modern toolchains like uv and ruff and addresses cutting-edge hardware architecture.

**Source:** [NVIDIA/Isaac-GR00T/CLAUDE.md](https://github.com/NVIDIA/Isaac-GR00T/blob/65cc4a192e6d084650d97747308b6a8deb790722/CLAUDE.md) · 7337★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Isaac GR00T N1.7

## Project overview

Isaac GR00T N1.7 is an open vision-language-action (VLA) model for generalized humanoid robot skills.
The repo contains the model, training pipeline, evaluation harness, and deployment tooling.

- **Language:** Python 3.10 (dGPU, Orin); Python 3.12 (Thor, DGX Spark — see deployment dir)
- **Package manager:** [uv](https://docs.astral.sh/uv/)
- **Build system:** setuptools (see `pyproject.toml`)
- **CI:** internal GitLab CI (`.gitlab-ci.yml` + includes under `ci/`, not shipped to the public GitHub EA repo); public GitHub Actions (`.github/workflows/`)

## Quick-start commands

```bash
# Install (dev mode with all extras)
uv sync --all-extras

# Lint and format (uses ruff via pre-commit)
pre-commit run --all-files

# Run CPU tests
python -m pytest tests/ -m "not gpu" -v --timeout=300

# Run GPU tests
python -m pytest tests/ -m gpu -v --timeout=300

# Build package
uv build

# Validate lockfile
uv lock --locked
```

## Code style

- Formatter: `ruff format` (double quotes, spaces, line-length 100)
- Linter: `ruff check` with rules E, F, I (ignores E501)
- Config lives in `pyproject.toml` under `[tool.ruff]`
- Run `pre-commit run --a
```

</details>
