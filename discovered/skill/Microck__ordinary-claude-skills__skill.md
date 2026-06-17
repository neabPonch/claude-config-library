---
name: Microck__ordinary-claude-skills__skill
source: https://github.com/Microck/ordinary-claude-skills/blob/8f5c83174f7aa683b4ddc7433150471983b93131/skills_categorized/education/hypogenic/SKILL.md
repo: Microck/ordinary-claude-skills
kind: skill
stars: 237
last_pushed: 2026-04-30T19:30:43Z
license: other
score: 8
domains: [agents-ai, scientific-research, data-science]
tags: [hypothesis-generation, llm-research, automated-discovery]
curated: 2026-06-17
curated_by: config-scout
---

# Microck/ordinary-claude-skills — skill

**Why it's worth keeping:** The highly structured YAML configuration templates (with variable injection) and strict JSON dataset schemas provide excellent patterns for delegating complex research tasks to agents.

**Summary:** A framework for automated scientific hypothesis generation and testing by integrating empirical data with literature-based insights via LLMs.

**Source credibility:** High; developed by a specialized research group (ChicagoHAI) with notable GitHub star count.

**Recency:** Current; utilizes modern toolchains like 'uv' and focuses on contemporary agentic workflows.

**Source:** [Microck/ordinary-claude-skills/skills_categorized/education/hypogenic/SKILL.md](https://github.com/Microck/ordinary-claude-skills/blob/8f5c83174f7aa683b4ddc7433150471983b93131/skills_categorized/education/hypogenic/SKILL.md) · 237★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: hypogenic
description: Automated hypothesis generation and testing using large language models. Use this skill when generating scientific hypotheses from datasets, combining literature insights with empirical data, testing hypotheses against observational data, or conducting systematic hypothesis exploration for research discovery in domains like deception detection, AI content detection, mental health analysis, or other empirical research tasks.
---

# Hypogenic

## Overview

Hypogenic provides automated hypothesis generation and testing using large language models to accelerate scientific discovery. The framework supports three approaches: HypoGeniC (data-driven hypothesis generation), HypoRefine (synergistic literature and data integration), and Union methods (mechanistic combination of literature and data-driven hypotheses).

## Quick Start

Get started with Hypogenic in minutes:

```bash
# Install the package
uv pip install hypogenic

# Clone example datasets
git clone https://github.com/ChicagoHAI/HypoGeniC-datasets.git ./data

# Run basic hypothesis generation
hypogenic_generation --config ./data/your_task/config.yaml --method hypogenic --num_hypotheses 20

# Run i
```

</details>
