---
name: Zenobia000__OpenCV-tools-image-process
source: https://github.com/Zenobia000/OpenCV-tools-image-process/blob/8ce6e1a5fabaa623bc8fca0bcdbac8134bf4c586/CLAUDE.md
repo: Zenobia000/OpenCV-tools-image-process
kind: claude-md
stars: 13
last_pushed: 2025-10-15T02:34:11Z
license: mit
score: 8
domains: [computer-vision, python]
tags: [opencv, structured-hierarchy, migration-strategy]
curated: 2026-06-16
curated_by: config-scout
---

# Zenobia000/OpenCV-tools-image-process — claude-md

**Why it's worth keeping:** Provides high-density structural context, exact import conventions, and clear success/performance targets to guide autonomous agent reasoning during refactoring or development.

**Summary:** Establishes a detailed modular hierarchy and specific file migration mappings alongside environment verification commands.

**Source credibility:** Small educational repository with highly organized, professional documentation structure.

**Recency:** Very current; explicitly references Claude Code and uses modern Python workflows.

**Source:** [Zenobia000/OpenCV-tools-image-process/CLAUDE.md](https://github.com/Zenobia000/OpenCV-tools-image-process/blob/8ce6e1a5fabaa623bc8fca0bcdbac8134bf4c586/CLAUDE.md) · 13★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an **OpenCV Computer Vision Toolkit** - a comprehensive learning platform for computer vision and image processing. The project is designed as an educational resource with modular architecture, progressing from fundamentals to advanced applications.

**Core Purpose**: Build a modern computer vision learning toolkit with 345+ test images, pre-trained models, and real-world project implementations.

## Development Commands

### Environment Setup
```bash
# Create and activate virtual environment
python -m venv cv_env
source cv_env/bin/activate  # Linux/Mac
# cv_env\Scripts\activate  # Windows

# Install dependencies
pip install -r requirements.txt

# Verify installation
python -c "import cv2, numpy as np; from utils import image_utils; print('✅ Setup complete')"
```

### Jupyter Development
```bash
# Start Jupyter Lab for development
jupyter lab

# Install additional widgets if needed
pip install jupyterlab
jupyter labextension install @jupyterlab/widgets
```

### Testing and Quality
```bash
# Run tests (when implemented)
pytest

# Code form
```

</details>
