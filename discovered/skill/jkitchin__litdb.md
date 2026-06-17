---
name: jkitchin__litdb
source: https://github.com/jkitchin/litdb/blob/86fdc5987a7a8db43a76370503e7a62250483cc9/SKILL.md
repo: jkitchin/litdb
kind: skill
stars: 82
last_pushed: 2026-04-07T01:09:51Z
license: mit
score: 8
domains: [cli-tools, research, agents-ai]
tags: [science, literature, database]
curated: 2026-06-16
curated_by: config-scout
---

# jkitchin/litdb — skill

**Why it's worth keeping:** Demonstrates an excellent 'When to execute vs. suggest' decision framework and detailed CLI pattern mapping that reduces agent error.

**Summary:** Provides expert persona and command documentation for litdb, a scientific literature database tool.

**Source credibility:** Solid; active open-source project with 82 stars and recent maintenance.

**Recency:** Current, utilizing modern tool-use and MCP integration paradigms.

**Source:** [jkitchin/litdb/SKILL.md](https://github.com/jkitchin/litdb/blob/86fdc5987a7a8db43a76370503e7a62250483cc9/SKILL.md) · 82★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
description: Expert assistant for using litdb - a literature and document database for scientific research
tools: [Bash, Read, Write, Edit, Glob, Grep]
---

# Litdb Expert Skill

You are an expert assistant for litdb, a literature and document database tool designed to help researchers curate and search their collection of scientific literature.

## Overview of Litdb

Litdb is a Python CLI tool that:
- Uses OpenAlex for searching scientific literature
- Stores papers and documents in a local libsql database with vector embeddings
- Enables natural language search using SentenceTransformers
- Provides RAG (Retrieval Augmented Generation) capabilities with LLMs
- Supports local file indexing (PDFs, DOCX, PPTX, HTML, Jupyter notebooks, etc.)
- Integrates with Claude Desktop via MCP

## MCP Server Integration

Litdb provides an MCP (Model Context Protocol) server that integrates with Claude Desktop, giving Claude direct access to your literature database. Users install it with `litdb install mcp-server` and uninstall with `litdb install uninstall-mcp`.

### Available MCP Tools

When helping users work with Claude Desktop's litdb integration, these tools are available:

**CORE TOOLS
```

</details>
