---
name: UABPeriopAI__Templates
source: https://github.com/UABPeriopAI/Templates/blob/1230ffa4d9a3002e1a0d7cb87d7acc0dc8df925c/CLAUDE.md
repo: UABPeriopAI/Templates
kind: claude-md
stars: 19
last_pushed: 2026-06-08T20:49:13Z
license: other
score: 9
domains: [mlops, signal-processing, python, data-science]
tags: [architecture, state-machine, command-reference, security-rules]
curated: 2026-06-15
curated_by: config-scout
---

# UABPeriopAI/Templates — claude-md

**Why it's worth keeping:** It uses text-based visual diagrams to explain control flow/state machines and enforces a 'reuse before writing' rule to prevent code duplication across submodules.

**Summary:** This file provides an exhaustive architectural blueprint of a complex MLOps pipeline, including state machine transitions and data flow logic. It serves as a masterclass in guiding an AI through specialized software patterns.

**Source credibility:** Highly credible; authored by a specialized perioperative data science team at UAB with active maintenance.

**Recency:** 

**Source:** [UABPeriopAI/Templates/CLAUDE.md](https://github.com/UABPeriopAI/Templates/blob/1230ffa4d9a3002e1a0d7cb87d7acc0dc8df925c/CLAUDE.md) · 19★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

NCVV (Neurocritical Care Vitals Variability) is an MLOps-oriented signal processing pipeline for high-resolution physiological waveform analysis (ECG, ABP, ICP). It provides a CLI (Typer) for batch processing, a Streamlit web UI, and a Gradio web UI for interactive use. The pipeline extracts per-beat features, applies quality control, and computes windowed variability metrics (HRV, BPV, ICPV), with experiment tracking via MLflow.

## Commands

```bash
# Setup (creates venv, installs deps including git submodule)
make venv

# Run the Qt desktop app (PySide6, primary)
make qt
# or: uv run --extra qt python -m app.qt

# Run the Streamlit UI (secondary)
uv run streamlit run NCVV/new_ui.py

# Run the Gradio UI (secondary)
uv run python NCVV/gradio_state_machine.py

# CLI — preprocess raw waveforms
uv run python NCVV/main.py preprocess-data --test-run True

# CLI — QC only (on preprocessed signals)
uv run python NCVV/main.py qc-only --test-run True

# CLI — full processing (extract + QC + visualization)
uv run python NCVV/main.py process-data --test-ru
```

</details>
