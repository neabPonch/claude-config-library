---
name: ryanmcafee__homelab
source: https://github.com/ryanmcafee/homelab/blob/916c77ba11b15e188a05ba0f64ea986ec950636d/Claude.md
repo: ryanmcafee/homelab
kind: claude-md
stars: 0
last_pushed: 2026-06-13T20:00:48Z
license: mit
score: 9
domains: [devops, kubernetes, agents-ai, infrastructure-as-code]
tags: [subagents, mcp, memory-management, tool-routing, gitops]
curated: 2026-06-15
curated_by: config-scout
---

# ryanmcafee/homelab — claude-md

**Why it's worth keeping:** The 'Tool Routing' table (enforcing specific retrieval tools over grep) and the 'Three-Tier Memory System' are elite, transferable strategies for managing context and agent learning. The subagent parallelization patterns provide a perfect blueprint for complex multi-step task execution.

**Summary:** This file establishes a sophisticated orchestration layer using specialized subagent routing and a highly structured three-tier memory system. It provides strict tool-routing rules to optimize discovery through LSP-first patterns rather than generic searches.

**Source credibility:** High-quality technical content likely from an expert in GitOps/Kubernetes despite low repo stars.

**Recency:** Extremely current; demonstrates advanced usage of MCP and Claude Code's memory mechanisms.

**Source:** [ryanmcafee/homelab/Claude.md](https://github.com/ryanmcafee/homelab/blob/916c77ba11b15e188a05ba0f64ea986ec950636d/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Homelab Project - Claude AI Instructions

Read `AGENTS.md` and apply the rules to all subagents.
When implementing plans, always analyze the plan first and look for opportunities to use sub agents.
Before implementing a plan, ensure that 'bd' is used for task tracking to support saving progress and context for long running tasks.

## Allowed Tools

Tool routing is mandatory, not advisory. Grep/Glob/Read are fallback tools. Every code-exploration session MUST start with `mcp__serena__list_memories` and `mcp__serena__get_symbols_overview` for the relevant files. Using Grep before `search_for_pattern`, or Read before `get_symbols_overview` on a code file, is a bug. Exceptions: non-code assets (YAML values files, plain Markdown, raw HCL), binary output, and files in languages without LSP support.

### Serena Tool Routing

| Task | Use Serena | Instead of |
|------|-----------|------------|
| Regex search with context | `search_for_pattern` | Grep |
| File discovery (.gitignore aware) | `find_file` / `list_dir` | Glob |
| Navigate Go/TS code | `find_symbol` / `get_symbols_overview` | Grep + Read |
| Trace function usage | `find_referencing_symbols` | Grep |
| Persist agent learnings |
```

</details>
