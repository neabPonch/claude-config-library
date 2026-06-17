---
name: kitzeslab__bioacoustics-model-zoo
source: https://github.com/kitzeslab/bioacoustics-model-zoo/blob/dd3e399e44c4aae6dfbba2807e222d713b847501/CLAUDE.md
repo: kitzeslab/bioacoustics-model-zoo
kind: claude-md
stars: 66
last_pushed: 2026-05-03T03:21:40Z
license: mit
score: 8
domains: [machine-learning, data-science, python]
tags: [model-zoo, dependency-management, research-framework]
curated: 2026-06-15
curated_by: config-scout
---

# kitzeslab/bioacoustics-model-zoo — claude-md

**Why it's worth keeping:** It includes a step-by-step 'Adding New Models' recipe and explains conditional import patterns to prevent Claude from assuming all dependencies are present.

**Summary:** This file provides comprehensive command instructions alongside detailed architectural mappings for model registration and optional dependency management.

**Source credibility:** Moderate; 66 stars indicates a specialized scientific research tool with recent maintenance.

**Recency:** Current; utilizes modern Python packaging (Poetry) and testing patterns.

**Source:** [kitzeslab/bioacoustics-model-zoo/CLAUDE.md](https://github.com/kitzeslab/bioacoustics-model-zoo/blob/dd3e399e44c4aae6dfbba2807e222d713b847501/CLAUDE.md) · 66★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Common Development Commands

### Testing
- `pytest` - Run all tests (tests are in the `tests/` directory)
- `pytest tests/test_birdnet.py` - Run specific model tests

### Code Formatting  
- `black .` - Format code with Black formatter (configured in pyproject.toml)
- `black --check .` - Check formatting without making changes

### Package Management
- `poetry install` - Install dependencies using Poetry
- `poetry add <package>` - Add new dependency
- `pip install -e .` - Install package in development mode

### BirdSet Subproject (in src/birdset/)
- `python train.py` - Train BirdSet models using Hydra configs
- `python eval.py` - Evaluate trained models
- `python eval.py experiment=local/DT_example` - Run specific experiment configs

## Project Architecture

### High-Level Structure
This is a bioacoustics model zoo that provides pre-trained models for bird and other animal sound classification. The repository contains two main components:

1. **Main Model Zoo** (`bioacoustics_model_zoo/`) - Collection of wrapped pre-trained models with unified API
2. **BirdSet In
```

</details>
