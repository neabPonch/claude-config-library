---
name: open-experiments__Telco-AIX
source: https://github.com/open-experiments/Telco-AIX/blob/ecf5099de9c2e712a22b16e9798f2d2f4bee89cb/CLAUDE.md
repo: open-experiments/Telco-AIX
kind: claude-md
stars: 219
last_pushed: 2026-04-24T13:43:51Z
license: mit
score: 8
domains: [agents-ai, machine-learning]
tags: [multi-project, protocol-driven, execution-context]
curated: 2026-06-15
curated_by: config-scout
---

# open-experiments/Telco-AIX — claude-md

**Why it's worth keeping:** Excells at mapping specific directories to their unique run commands and explaining custom internal protocols (MCP/ACP) to guide agentic reasoning.

**Summary:** Provides essential execution and architectural guidance for a collection of independent AI sub-projects. It prevents the AI from searching for non-existent global build systems by defining project-specific entry points.

**Source credibility:** 219 stars indicates a recognized, specialized repository for telecommunications AI experiments.

**Recency:** 

**Source:** [open-experiments/Telco-AIX/CLAUDE.md](https://github.com/open-experiments/Telco-AIX/blob/ecf5099de9c2e712a22b16e9798f2d2f4bee89cb/CLAUDE.md) · 219★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

Telco-AIX is a collection of independent AI/ML experiment projects for the telecommunications domain. Each subdirectory is a self-contained project with its own dependencies — there is no monorepo build system, shared library, or CI/CD pipeline.

Models and datasets are published to HuggingFace: `huggingface.co/collections/fenar/telco-aix-66737384ab5687fe3d9a4b94`

## Running Projects

Each project is independent. The general pattern is:

```bash
cd <project-dir>
pip install -r requirements.txt
python main.py  # or the project's entry script
```

**agentic/** and **autonet/** (multi-agent frameworks):
```bash
pip install -r requirements.txt
python main.py          # starts MCP (port 8000), ACP broker (8002), dashboard (8080)
python main.py --run-test  # agentic: runs with test scenario
```

**telco-sme/** (Gradio UI):
```bash
pip install -r requirements-v2.txt
python sme-web-ui-v2.py
```

**5gprod/** (Dash dashboard), **crm/** (Flask), **churn/** (Flask server on port 5000), **revenueassurance/** (Flask): each has a main Python script that sta
```

</details>
