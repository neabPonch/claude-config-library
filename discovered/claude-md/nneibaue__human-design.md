---
name: nneibaue__human-design
source: https://github.com/nneibaue/human-design/blob/afe0acc1d35478ad7505e4c6e4a8fd3204b88d45/CLAUDE.md
repo: nneibaue/human-design
kind: claude-md
stars: 0
last_pushed: 2026-06-14T16:38:42Z
license: unknown
score: 9
domains: [cli-tools, backend-api, data-science]
tags: [python, architectural-patterns, dev-container, workflow-optimization]
curated: 2026-06-15
curated_by: config-scout
---

# nneibaue/human-design — claude-md

**Why it's worth keeping:** It includes specific 'anti-documentation' rules to prevent AI file clutter, outlines high-level architectural patterns (Separation of Concerns), and documents critical API quirks that would otherwise cause logical errors.

**Summary:** Combines technical environment setup with deep architectural principles and human-centric workflow priorities. It provides a clear roadmap for maintaining the separation of raw astronomical calculations from semantic layers.

**Source credibility:** Low star count suggests a niche or private project, but the technical depth implies professional-grade engineering.

**Recency:** Highly current; utilizes cutting-edge Python versions and modern tooling like Pydantic v2 and Ruff.

**Source:** [nneibaue/human-design/CLAUDE.md](https://github.com/nneibaue/human-design/blob/afe0acc1d35478ad7505e4c6e4a8fd3204b88d45/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Python toolkit for Human Design built for Rebecca Jolli of Jolly Alchemy. This project calculates Human Design bodygraphs from birth information using astronomical calculations. The core calculation system is intentionally agnostic of any specific semantic description system (Ra Uru Hu's traditional system, 64keys terminology, or future custom naming).

**Key architectural principle**: Separate raw astronomical calculations from semantic overlays. Raw models (gate numbers, planetary positions, coordinate ranges) should never assume a particular interpretation system.

The project embodies "Rebecca Energy" - whimsical yet grounded, warm and approachable, focusing on self-discovery and deconditioning.

## Development Environment

### Working in Dev Container (Preferred)
This project uses a dev container for consistent development environments:

- **Dockerfile**: Multi-stage build with `development` target
- **Python version**: 3.14 (bookworm base)
- **Container user**: Matches host user (passed via `${localEnv:USER}`)
- **Dependencies**: Installed
```

</details>
