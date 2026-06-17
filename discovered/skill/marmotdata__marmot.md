---
name: marmotdata__marmot
source: https://github.com/marmotdata/marmot/blob/78db528688c2b4fdc590f17fb266c96c7757f589/SKILL.md
repo: marmotdata/marmot
kind: skill
stars: 576
last_pushed: 2026-06-09T09:28:37Z
license: mit
score: 9
domains: [data-engineering, cli-tools, agents-ai]
tags: [data-catalog, mcp, infrastructure]
curated: 2026-06-14
curated_by: config-scout
---

# marmotdata/marmot — skill

**Why it's worth keeping:** It defines an explicit tool-selection hierarchy (Prefer MCP > Fallback to CLI/API) and includes actionable JSON configuration blocks for agent setup.

**Summary:** A comprehensive skill file providing detailed instructions for interacting with a data catalog via MCP, CLI, and REST API.

**Source credibility:** High; the source is a well-starred, actively maintained infrastructure project.

**Recency:** Current; it specifically leverages the Model Context Protocol (MCP).

**Source:** [marmotdata/marmot/SKILL.md](https://github.com/marmotdata/marmot/blob/78db528688c2b4fdc590f17fb266c96c7757f589/SKILL.md) · 576★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: marmot
description: Interact with a Marmot data catalog instance. Use this skill when the user wants to search for data assets, view lineage, browse glossary terms, check pipeline runs, manage tags or owners, view metrics, or do anything related to their data catalog. Covers the Marmot CLI, REST API and MCP server.
---

This skill helps you interact with a Marmot data catalog. Marmot catalogs data assets (databases, tables, topics, APIs, dashboards) across an organisation's data stack and tracks lineage between them.

## Setup

The user needs the Marmot CLI installed and authenticated. If not already set up:

```bash
curl -fsSL get.marmotdata.io | sh
marmot login https://marmot.example.com
```

`marmot login` opens a browser for OAuth 2.0 PKCE authentication and caches the token locally. Alternatively, use an API key:

```bash
export MARMOT_HOST=https://marmot.example.com
export MARMOT_API_KEY=<key>
```

Or pass `--host` and `--api-key` as flags on any command.

## MCP Server

Marmot has a built-in MCP (Model Context Protocol) server. If the user has configured MCP, you can interact with the catalog directly using these tools instead of the CLI:

- **discover_data** — uni
```

</details>
