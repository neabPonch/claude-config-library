---
name: Anemll__Anemll
source: https://github.com/Anemll/Anemll/blob/fb42f60b2e7a7b4709052c7146d37480bf21941e/CLAUDE.md
repo: Anemll/Anemll
kind: claude-md
stars: 1616
last_pushed: 2026-03-10T21:53:23Z
license: unknown
score: 9
domains: [machine-learning, mlops, ios]
tags: [ane, coreml, llm-optimization]
curated: 2026-06-15
curated_by: config-scout
---

# Anemll/Anemll — claude-md

**Why it's worth keeping:** The file includes highly specific 'CRITICAL' implementation rules regarding RMSNorm and KV-cache slicing that prevent subtle runtime failures on specialized hardware—rules an LLM would otherwise likely hallucinate or miss.

**Summary:** Provides a comprehensive technical guide for developing machine learning tools optimized for Apple's Neural Engine (ANE). It covers environment setup, conversion pipelines, and critical low-level hardware constraints.

**Source credibility:** High; the project has significant community interest with 1600+ stars and recent activity.

**Recency:** Highly current, explicitly mentioning Llama-3.1 and modern conversion workflows.

**Source:** [Anemll/Anemll/CLAUDE.md](https://github.com/Anemll/Anemll/blob/fb42f60b2e7a7b4709052c7146d37480bf21941e/CLAUDE.md) · 1616★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ANEMLL (pronounced "animal") is an open-source project for accelerating Large Language Models (LLMs) on Apple Neural Engine (ANE). The project converts Hugging Face models to CoreML format for on-device inference on Apple devices.

## Command Allowlist (Claude Code)

Approved commands for Claude Code in this repo:
```bash
osascript -e 'tell application "System Events" to key code 121'  # page down
sleep 0.5
export ANEMLL_HOST="http://127.0.0.1:8765"
curl ...
```

## Development Commands

### Environment Setup
```bash
# Create Python 3.9 virtual environment (required)
python -m venv anemll-env
source anemll-env/bin/activate
pip install -r requirements.txt

# Install Xcode Command Line Tools (required for CoreML compilation)
xcode-select --install
xcrun --find coremlcompiler  # Verify installation
```

**Important**: Always activate the virtual environment before running any Python scripts in this repository:
```bash
source env-anemll/bin/activate  # or anemll-env/bin/activate depending on your setup
```

You can verify the environment is active by
```

</details>
