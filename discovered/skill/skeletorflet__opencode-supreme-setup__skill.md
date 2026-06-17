---
name: skeletorflet__opencode-supreme-setup__skill
source: https://github.com/skeletorflet/opencode-supreme-setup/blob/f932a5312f15194cfe6f97aa6a39b8ec7f842c8d/.claude/skills/graphify/skill.md
repo: skeletorflet/opencode-supreme-setup
kind: skill
stars: 46
last_pushed: 2026-05-20T14:32:45Z
license: mit
score: 9
domains: [cli-tools, knowledge-graphs, developer-experience]
tags: [graphrag, codebase-analysis, knowledge-engine]
curated: 2026-06-15
curated_by: config-scout
---

# skeletorflet/opencode-supreme-setup — skill

**Why it's worth keeping:** Implements an excellent 'fast path' logic where the agent checks for existing graph state to avoid redundant extraction; provides highly detailed instructions for complex workflows like cross-repo merging.

**Summary:** Converts codebases or documentation into an interactive knowledge graph for semantic querying and structural analysis.

**Source credibility:** Niche popularity with 46 stars and recent maintenance (1 month ago).

**Recency:** Very current, specifically optimized for modern agentic tool usage/Claude Code.

**Source:** [skeletorflet/opencode-supreme-setup/.claude/skills/graphify/skill.md](https://github.com/skeletorflet/opencode-supreme-setup/blob/f932a5312f15194cfe6f97aa6a39b8ec7f842c8d/.claude/skills/graphify/skill.md) · 46★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: graphify
description: "any input (code, docs, papers, images, videos) to knowledge graph. Use when user asks any question about a codebase, documents, or project content - especially if graphify-out/ exists, treat the question as a /graphify query."
trigger: /graphify
---

# /graphify

Turn any folder of files into a navigable knowledge graph with community detection, an honest audit trail, and three outputs: interactive HTML, GraphRAG-ready JSON, and a plain-language GRAPH_REPORT.md.

## Usage

```
/graphify                                             # full pipeline on current directory → Obsidian vault
/graphify <path>                                      # full pipeline on specific path
/graphify https://github.com/<owner>/<repo>           # clone repo then run full pipeline on it
/graphify https://github.com/<owner>/<repo> --branch <branch>  # clone a specific branch
/graphify <url1> <url2> ...                           # clone multiple repos, build each, merge into one cross-repo graph
/graphify <path> --mode deep                          # thorough extraction, richer INFERRED edges
/graphify <path> --update                             # incremental - re-extract onl
```

</details>
