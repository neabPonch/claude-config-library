---
name: HarleyCoops__Math-To-Manim__claude
source: https://github.com/HarleyCoops/Math-To-Manim/blob/8915ea06fc9844e1607b920df7df59cc9885d96e/legacy/Math-To-Manim/CLAUDE.md
repo: HarleyCoops/Math-To-Manim
kind: claude-md
stars: 2390
last_pushed: 2026-06-14T16:47:41Z
license: unknown
score: 9
domains: [agents-ai, mathematics, python]
tags: [agentic-workflow, manim, knowledge-graphs, data-structures]
curated: 2026-06-17
curated_by: config-scout
---

# HarleyCoops/Math-To-Manim — claude-md

**Why it's worth keeping:** Includes critical data structures (KnowledgeNode) and domain-specific syntax rules (LaTeX raw strings) that prevent common runtime errors. The architectural flowchart gives Claude a mental model of the multi-agent orchestration.

**Summary:** Provides a high-level conceptual framework of the 'reverse knowledge tree' alongside specific technical constraints for Manim and LaTeX. It effectively bridges agent logic with implementation details.

**Source credibility:** High; 2k+ stars and recent activity suggest a well-maintained, high-quality specialized repository.

**Recency:** Current; reflects modern agentic patterns and specific tool dependency requirements.

**Source:** [HarleyCoops/Math-To-Manim/legacy/Math-To-Manim/CLAUDE.md](https://github.com/HarleyCoops/Math-To-Manim/blob/8915ea06fc9844e1607b920df7df59cc9885d96e/legacy/Math-To-Manim/CLAUDE.md) · 2390★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Math-To-Manim transforms simple prompts like "explain cosmology" into professional Manim Community Edition animations using a multi-agent system based on **reverse knowledge tree decomposition**. The core innovation: recursively asking "What must I understand BEFORE X?" to build pedagogically sound animations from foundation concepts up to advanced topics.

**Three AI pipelines**: Claude (Anthropic SDK), Gemini 3 (Google ADK), Kimi K2.5 (Moonshot)

## Repository Structure

```
Math-To-Manim/
├── src/                    # Claude pipeline
│   ├── agents/             # Agent implementations
│   │   ├── prerequisite_explorer.py  # Unified explorer with pluggable clients
│   │   ├── orchestrator.py           # Full pipeline orchestrator
│   │   ├── narrative_composer.py     # Tree -> verbose prompt
│   │   └── threejs_code_generator.py # Three.js output
│   ├── app.py              # DeepSeek Gradio UI
│   └── app_claude.py       # Claude Gradio UI
├── Gemini3/                # Google Gemini 3 pipeline
├── KimiK2.5Swarm/          # Kimi K2.5 Swarm pipe
```

</details>
