---
name: Yuan1z0825__nature-skills__skill
source: https://github.com/Yuan1z0825/nature-skills/blob/3f33129f6b3c7f9ee9a42d8d4c31168f5f5d2676/skills/nature-figure/SKILL.md
repo: Yuan1z0825/nature-skills
kind: skill
stars: 20074
last_pushed: 2026-06-14T13:51:54Z
license: mit
score: 9
domains: [data-visualization, scientific-computing, agent-orchestration]
tags: [workflow-automation, academic-plotting, context-management, rag-style-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# Yuan1z0825/nature-skills — skill

**Why it's worth keeping:** The architectural pattern of using a short router to dynamically load specialized fragments is a masterclass in managing large-scale agentic instructions within token limits. The 'blocking gate' approach for backend selection ensures high precision and minimizes irrelevant library loading.

**Summary:** A sophisticated router skill that orchestrates high-impact scientific figure generation through a multi-layered 'router-fragment-reference' architecture. It uses a strict gatekeeper protocol to select between Python and R backends to prevent context bloat.

**Source credibility:** High; the repository is highly starred and demonstrates professional-grade structural design for academic workflows.

**Recency:** Current; specifically optimized for modern LLM context management and tool-use efficiency.

**Source:** [Yuan1z0825/nature-skills/skills/nature-figure/SKILL.md](https://github.com/Yuan1z0825/nature-skills/blob/3f33129f6b3c7f9ee9a42d8d4c31168f5f5d2676/skills/nature-figure/SKILL.md) · 20074★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: nature-figure
description: >-
  Submission-grade Nature/high-impact journal figure workflow for Python or R. Use whenever the user asks to create, revise, audit, or polish manuscript figures, multi-panel scientific plots, figures4papers-style matplotlib plots, or journal-ready SVG/PDF/TIFF outputs, especially for Nature-family or other high-impact journals. Before plotting, define the figure's conclusion, evidence logic, export needs, and review risks. If the user has not chosen Python or R, ask "Python or R?" and stop. Use only the selected backend for figure generation, previewing, exporting, and QA. Supports matplotlib/seaborn and ggplot2/patchwork/ComplexHeatmap. Not for dashboards or Illustrator/Figma-first infographics. Also trigger on general academic-writing figure needs even without the word "Nature", such as making figures/plots for a paper, scientific/academic plotting, data visualization for a manuscript, and Chinese phrasings like 论文配图、学术写作配图、科研绘图、科研作图、画图、作图、出图、论文图表、可视化.
version: 2.0.0
author: Community contribution, refactored into static/dynamic layers
---

# Nature Figure Making — Router

This skill is split into two layers:

- A **static layer** under `st
```

</details>
