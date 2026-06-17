---
name: pinecone-io__pinecone-claude-code-plugin__skill
source: https://github.com/pinecone-io/pinecone-claude-code-plugin/blob/9af99dc1dc10ce291ec67dc51d46199544a0cd4f/skills/query/SKILL.md
repo: pinecone-io/pinecone-claude-code-plugin
kind: skill
stars: 67
last_pushed: 2026-05-26T20:31:29Z
license: mit
score: 8
domains: [vector-databases, ai-agents, cli-tools]
tags: [pinecone, mcp, search, embeddings]
curated: 2026-06-15
curated_by: config-scout
---

# pinecone-io/pinecone-claude-code-plugin — skill

**Why it's worth keeping:** Uses highly effective 'negative constraints' to prevent incorrect tool usage and a proactive discovery workflow that utilizes secondary tools to resolve missing user arguments.

**Summary:** Provides structured instructions for querying Pinecone integrated indexes via MCP, emphasizing prerequisites and tool-based discovery.

**Source credibility:** High; official documentation from the Pinecone engineering team.

**Recency:** Current, specifically tailored for MCP-enabled agentic workflows in Claude Code.

**Source:** [pinecone-io/pinecone-claude-code-plugin/skills/query/SKILL.md](https://github.com/pinecone-io/pinecone-claude-code-plugin/blob/9af99dc1dc10ce291ec67dc51d46199544a0cd4f/skills/query/SKILL.md) · 67★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pinecone:query
description: Query integrated indexes using text with Pinecone MCP. IMPORTANT - This skill ONLY works with integrated indexes (indexes with built-in Pinecone embedding models like multilingual-e5-large). For standard indexes or advanced vector operations, use the CLI skill instead. Requires PINECONE_API_KEY environment variable and Pinecone MCP server to be configured.
argument-hint: query [q] index [indexName] namespace [ns] topK [k] reranker [rerankModel]
allowed-tools: Bash, Read
---

# Pinecone Query Skill

Search for records in Pinecone integrated indexes using natural language text queries via the Pinecone MCP server.

## What is this skill for?

This skill provides a simple way to query **integrated indexes** (indexes with built-in Pinecone embedding models) using text queries. The MCP server automatically converts your text into embeddings and searches the index.

### Prerequisites

**Required:**
1. ✅ **Pinecone MCP server must be configured** - Check if MCP tools are available
2. ✅ **PINECONE_API_KEY environment variable must be set** - Get a free API key at https://app.pinecone.io/?sessionType=signup
3. ✅ **Index must be an integrated index** - Us
```

</details>
