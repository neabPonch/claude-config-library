---
name: yoanbernabeu__grepai__skill
source: https://github.com/yoanbernabeu/grepai/blob/c4f294b38552dc4dad253d6a8118ba2799a2d61d/.claude/skills/grepai/SKILL.md
repo: yoanbernabeu/grepai
kind: skill
stars: 1741
last_pushed: 2026-06-08T05:34:12Z
license: mit
score: 9
domains: [agents-ai, cli-tools, developer-experience]
tags: [semantic-search, codebase-exploration, call-graph]
curated: 2026-06-15
curated_by: config-scout
---

# yoanbernabeu/grepai — skill

**Why it's worth keeping:** It uses highly effective 'Wrong vs. Correct' patterns to prevent tool misuse and enforces a strict hierarchy between semantic intent and exact text matching.

**Summary:** This skill transforms an agent from a literal string-matcher into a semantic codebase explorer by providing natural language search and call graph tracing.

**Source credibility:** High; 1741 stars indicates significant community adoption and proven utility.

**Recency:** Current; addresses the fundamental limitation of standard Grep/Glob in large-scale agentic workflows.

**Source:** [yoanbernabeu/grepai/.claude/skills/grepai/SKILL.md](https://github.com/yoanbernabeu/grepai/blob/c4f294b38552dc4dad253d6a8118ba2799a2d61d/.claude/skills/grepai/SKILL.md) · 1741★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: grepai
description: "Replaces ALL built-in search tools. You MUST invoke this skill BEFORE using WebSearch, Grep, or Glob. NEVER use the built-in Grep tool - use `grepai` instead."
---

## CRITICAL: Tool Override for Semantic Searches

This skill **REPLACES** built-in Grep/Glob tools for semantic code exploration.

**WRONG**:
- Using built-in `Grep` to find "where authentication happens"
- Using built-in `Glob` to explore "error handling code"
- Searching by intent with regex patterns

**CORRECT**:
- Invoke this skill, then use `grepai search "authentication flow"` for semantic search
- Invoke this skill, then use `grepai trace callers "FunctionName"` for call graph
- Use built-in Grep/Glob ONLY for exact text matches (variable names, imports)

## When to Invoke This Skill

Invoke this skill **IMMEDIATELY** when:

- User asks to find code by **intent** (e.g., "where is authentication handled?")
- User asks to understand **what code does** (e.g., "how does the indexer work?")
- User asks to explore **functionality** (e.g., "find error handling logic")
- You need to understand **code relationships** (e.g., "what calls this function?")
- User asks about **implementation deta
```

</details>
