---
name: moinulmoin__ai-grep__claude-skill
source: https://github.com/moinulmoin/ai-grep/blob/766b4d19987ee875a07734cec86e1de23106b275/docs/CLAUDE_SKILL.md
repo: moinulmoin/ai-grep
kind: skill
stars: 6
last_pushed: 2026-02-07T18:45:12Z
license: mit
score: 8
domains: [cli-tools, agents-ai, developer-experience]
tags: [semantic-search, instructional-prompt, specialized-skill]
curated: 2026-06-16
curated_by: config-scout
---

# moinulmoin/ai-grep — skill

**Why it's worth keeping:** It includes actionable heuristics like synonym-based retries when scores are low and quantitative thresholds for result reliability. The logic of grouping queries by workflow is a highly transferable pattern for any semantic tool.

**Summary:** A specialized skill prompt that teaches Claude how to use the `ai-grep` CLI for semantic code search. It provides guidance on query iteration, score interpretation, and troubleshooting.

**Source credibility:** Low star count (6) but high signal-to-noise ratio in the instruction set.

**Recency:** Current; reflects modern local embedding/CLI patterns relevant to 2025 agentic workflows.

**Source:** [moinulmoin/ai-grep/docs/CLAUDE_SKILL.md](https://github.com/moinulmoin/ai-grep/blob/766b4d19987ee875a07734cec86e1de23106b275/docs/CLAUDE_SKILL.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ai-grep Skill for Claude (2025)

A skill prompt that teaches Claude Code how to use `ai-grep` effectively. Pair this with the existing MCP server to get both **hands (MCP tools)** and **brains (Skill guidance)**.

## How to load
Copy this Skill text into a Claude Project/Skill, or paste into a system message before your task. Keep it short and focused.

## When to use ai-grep vs ripgrep
- Use `ai-grep search "concept"` for semantic questions ("authentication flow", "error handling", "database connection pooling").
- Use `rg "literal"` (outside this skill) for exact strings, symbols, config keys.
- Prefer `--no-rerank` for speed-sensitive probes; default rerank for highest accuracy.

## Query strategy
- Start specific: "jwt verification handler" → good matches.
- If few results (<3) or low scores (<0.65): rewrite query with synonyms ("login", "auth", "token validation"), retry.
- For workflows: run 2–3 related queries ("auth middleware", "jwt validation", "session refresh") and merge.

## Command patterns
- Semantic search (JSON): `ai-grep search "authentication flow" --format json`
- Faster: `ai-grep search "auth" --format json --no-rerank`
- Pretty output (human review): `--form
```

</details>
