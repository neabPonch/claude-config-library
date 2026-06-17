---
name: sgarcese__Civic-Analytics-Agent-Workflow-Claude-Skill__benchmarking-skill
source: https://github.com/sgarcese/Civic-Analytics-Agent-Workflow-Claude-Skill/blob/a9ad881370d353dfb04076d36ef409b17cecba1c/Benchmarking_Skill.md
repo: sgarcese/Civic-Analytics-Agent-Workflow-Claude-Skill
kind: skill
stars: 36
last_pushed: 2026-04-02T17:50:05Z
license: mit
score: 9
domains: [agents-ai, data-analysis, civic-tech]
tags: [benchmarking, open-data, comparative-analysis, mcp]
curated: 2026-06-14
curated_by: config-scout
---

# sgarcese/Civic-Analytics-Agent-Workflow-Claude-Skill — skill

**Why it's worth keeping:** It enforces a 'schema-first' workflow to prevent query errors and includes a sophisticated reasoning framework (Comparability Assessment) to ensure data retrieved is actually comparable.

**Summary:** A specialized skill that enables a Claude agent to perform rigorous cross-city policy benchmarking by mapping specific tool protocols and comparative logic across municipal datasets.

**Source credibility:** High; the document demonstrates professional-grade data science rigor and domain expertise in civic analytics.

**Recency:** Very current; leverages specific MCP tool-calling patterns essential for Claude Code.

**Source:** [sgarcese/Civic-Analytics-Agent-Workflow-Claude-Skill/Benchmarking_Skill.md](https://github.com/sgarcese/Civic-Analytics-Agent-Workflow-Claude-Skill/blob/a9ad881370d353dfb04076d36ef409b17cecba1c/Benchmarking_Skill.md) · 36★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: city-benchmarking
description: "Use this skill whenever the user wants to compare Boston's performance to peer cities, identify best practices from other municipalities, understand how Boston ranks on any metric, or find evidence that a policy approach has worked elsewhere. ALWAYS use when the user mentions 'other cities', 'how does Boston compare', 'best practices', 'peer cities', 'what works', 'benchmarks', 'lessons from elsewhere', or asks whether Boston is doing better or worse than comparable municipalities. This skill uses Boston Open Data MCP (primary), San Francisco Open Data MCP (Socrata), Seattle Open Data MCP (Socrata), and DC Open Data MCP (ArcGIS) for rigorous cross-city comparisons against cities of comparable scale and complexity. Applies J-PAL caution to comparative claims and Bloomberg framing to translate benchmarks into actionable city policy recommendations. Includes a dedicated Performance Management Benchmarking module — pair with Performance_Management_Skill.md to compare cost-per-outcome, workload-per-FTE, and budget-efficiency ratios across all four cities."
---

# City Benchmarking — Cross-City Comparative Analysis

## Purpose and Power

Benchmar
```

</details>
