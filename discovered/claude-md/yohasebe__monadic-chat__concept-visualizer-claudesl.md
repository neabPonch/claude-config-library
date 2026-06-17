---
name: yohasebe__monadic-chat__concept-visualizer-claudesl
source: https://github.com/yohasebe/monadic-chat/blob/2aebb9498cc27120f76d643312e1d15e812dad73/docker/services/ruby/apps/concept_visualizer/concept_visualizer_claude.mdsl
repo: yohasebe/monadic-chat
kind: claude-md
stars: 69
last_pushed: 2026-06-14T10:11:23Z
license: apache-2.0
score: 9
domains: [agents-ai, visualization, tool-use]
tags: [latex, tikz, agentic-workflows, self-verification]
curated: 2026-06-15
curated_by: config-scout
---

# yohasebe/monadic-chat — claude-md

**Why it's worth keeping:** Contains advanced agentic patterns: the 'Plan-Approve-Execute' protocol and a 'Visual Self-Verification' loop to catch rendering errors.

**Summary:** Defines a high-agency system prompt for transforming concepts into LaTeX/TikZ diagrams via specific tool calls.

**Source credibility:** The source is an active, specialized project for local LLM orchestration.

**Recency:** 

**Source:** [yohasebe/monadic-chat/docker/services/ruby/apps/concept_visualizer/concept_visualizer_claude.mdsl](https://github.com/yohasebe/monadic-chat/blob/2aebb9498cc27120f76d643312e1d15e812dad73/docker/services/ruby/apps/concept_visualizer/concept_visualizer_claude.mdsl) · 69★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
app "ConceptVisualizerClaude" do
  icon "fa-solid fa-diagram-project"
  
  display_name "Concept Visualizer"
  description do
    en <<~TEXT
    Generate visual diagrams for concepts and relationships. <a href="https://yohasebe.github.io/monadic-chat/#/basic-usage/basic-apps?id=concept-visualizer" target="_blank"><i class="fa-solid fa-circle-info"></i></a>
    TEXT
    
    ja <<~TEXT
    概念と関係性の視覚的図表生成。 <a href="https://yohasebe.github.io/monadic-chat/#/basic-usage/basic-apps?id=concept-visualizer" target="_blank"><i class="fa-solid fa-circle-info"></i></a>
    TEXT
    
    zh <<~TEXT
    生成概念和关系的视觉图表。 <a href="https://yohasebe.github.io/monadic-chat/#/basic-usage/basic-apps?id=concept-visualizer" target="_blank"><i class="fa-solid fa-circle-info"></i></a>
    TEXT
    
    ko <<~TEXT
    개념과 관계의 시각적 다이어그램 생성. <a href="https://yohasebe.github.io/monadic-chat/#/basic-usage/basic-apps?id=concept-visualizer" target="_blank"><i class="fa-solid fa-circle-info"></i></a>
    TEXT
    
    es <<~TEXT
    Generar diagramas visuales para conceptos y relaciones. <a href="https://yohasebe.github.io/monadic-chat/#/basic-usage/basic-apps?id=concept-visualizer" target="_blank"><i class="fa-soli
```

</details>
