---
name: kerim__zotero-code-execution
source: https://github.com/kerim/zotero-code-execution/blob/9d521ef71dfda5fa8e8f5a5e63159dccbfdc7549/skill.md
repo: kerim/zotero-code-execution
kind: skill
stars: 57
last_pushed: 2026-01-20T13:54:23Z
license: mit
score: 9
domains: [agents-ai, data-analysis, knowledge-management]
tags: [search, zotero, orchestration, context-optimization]
curated: 2026-06-14
curated_by: config-scout
---

# kerim/zotero-code-execution — skill

**Why it's worth keeping:** Demonstrates the 'fetch-large/return-small' pattern to bypass context limits and solves complex query logic (like multi-term OR searches) within code rather than through repeated tool calls.

**Summary:** Implements a high-efficiency search pattern that uses Python code to fetch, filter, and rank large Zotero datasets locally before returning only the most relevant results to the LLM.

**Source credibility:** Solid community interest with 57 stars on GitHub and recent updates.

**Recency:** Up-to-date, specifically addressing semantic search adjustments from early 2025.

**Source:** [kerim/zotero-code-execution/skill.md](https://github.com/kerim/zotero-code-execution/blob/9d521ef71dfda5fa8e8f5a5e63159dccbfdc7549/skill.md) · 57★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: zotero-mcp-code
description: Search Zotero library using code execution for efficient multi-strategy searches without crash risks. Use this skill when the user needs comprehensive Zotero searches with automatic deduplication and ranking.
---

# Zotero MCP Code Execution Skill

Search your Zotero library using code execution for safe, efficient, comprehensive searches.

## 🎯 Core Concept

Instead of calling MCP tools directly (which loads all results into context and risks crashes), **write Python code** that:
1. Fetches large datasets (50-100+ items per strategy)
2. Filters and ranks in code execution environment
3. Returns only top N results to context

**Benefits:**
- ✅ No crash risk (large data stays in code)
- ✅ Automatic multi-strategy search
- ✅ Automatic deduplication
- ✅ Automatic ranking
- ✅ One function call instead of 5-10

## ⚠️ Critical Notes

### Multi-Term Searches
**Zotero treats multi-word queries as AND conditions!**

❌ **Wrong:** `comprehensive_search("Atyal Atayal 泰雅族")` → finds 0 results (needs ALL terms)
✅ **Right:** Search each term separately and merge results (see Pattern 6 below)

**When to use multi-term OR search:**
- Multiple spellings (Atayal
```

</details>
