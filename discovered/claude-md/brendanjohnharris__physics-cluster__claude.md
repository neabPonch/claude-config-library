---
name: brendanjohnharris__physics-cluster__claude
source: https://github.com/brendanjohnharris/physics-cluster/blob/a7cebe60b1330666bbb6304ec9c8bc13db942bf3/.claude/CLAUDE.md
repo: brendanjohnharris/physics-cluster
kind: claude-md
stars: 0
last_pushed: 2026-06-09T04:49:45Z
license: unknown
score: 8
domains: [scientific-computing, data-visualization, academic-writing]
tags: [julia, plotting, science, style-guide]
curated: 2026-06-16
curated_by: config-scout
---

# brendanjohnharris/physics-cluster — claude-md

**Why it's worth keeping:** The instructions excel at tool-use optimization (prioritizing MCP REPLs over terminal) and providing exhaustive visual specifications (color palettes/sizing) to ensure consistent, publication-ready figures.

**Summary:** A specialized configuration for Julia-based scientific research that includes strict plotting/theming standards and a sophisticated academic writing style guide.

**Source credibility:** Low public profile (0 stars), but the extreme specificity indicates a highly structured professional research workflow.

**Recency:** Current; includes modern Julia versioning and mentions MCPs used in contemporary agentic workflows.

**Source:** [brendanjohnharris/physics-cluster/.claude/CLAUDE.md](https://github.com/brendanjohnharris/physics-cluster/blob/a7cebe60b1330666bbb6304ec9c8bc13db942bf3/.claude/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AI instructions

## Global instructions
Please use em dashes (--- or unicode equivalent) sparingly; interjections are ok, but not so much if they close a sentence, where you shoudl prefer semicolons or colons (--- should typically be paired). NEVER put spaces around em dashes---always like this. Always be gramatically correct though.

## Coding

### Documentation and docstrings

Please use a slightly terse style for documentation, focusing on clarity and precision rather than hyping hte software.

### Julia language


#### Code evaluation

If you are considering running julia code in the terminal, especially if you are planning to write a new small script just to evaluate a small piece of code, please check if the Kaimon mcp is available, and if there is a connected repl for the current project. If so, please run code snippets there instead of the terminal.

#### Plotting

Please use CairoMakie as the plotting backend for all Julia code.
If the project you are working in has 'Fathom.jl' installed, please use 'Fathom.jl' for theming (it also has a number of recipes you should prefer over the CairoMakie defaults; e.g. prefer 'ziggurat' plots to 'hist' plots). This means `using Cair
```

</details>
