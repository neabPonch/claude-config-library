---
name: clidey__whodb__skill
source: https://github.com/clidey/whodb/blob/2af708d6a4d8464435e2b59c792bc6a9c34e63fa/cli/skills/whodb/SKILL.md
repo: clidey/whodb
kind: skill
stars: 4854
last_pushed: 2026-06-15T17:37:43Z
license: apache-2.0
score: 9
domains: [database, cli-tools, data-analysis]
tags: [sql, mcp, exploration]
curated: 2026-06-15
curated_by: config-scout
---

# clidey/whodb — skill

**Why it's worth keeping:** Includes highly tactical workflow examples that optimize tool calls (e.g., requesting columns during table listing) and provides specific CLI fallbacks for environment flexibility.

**Summary:** Provides end-to-end capabilities for database schema discovery, querying, and data export using both MCP tools and a robust CLI fallback.

**Source credibility:** High; the repository is well-starred (4.8k+) and actively maintained.

**Recency:** Current; aligns with modern MCP patterns used in Claude Code environments.

**Source:** [clidey/whodb/cli/skills/whodb/SKILL.md](https://github.com/clidey/whodb/blob/2af708d6a4d8464435e2b59c792bc6a9c34e63fa/cli/skills/whodb/SKILL.md) · 4854★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: whodb
description: Database operations including querying, schema exploration, and data analysis. Activates for tasks involving PostgreSQL, MySQL, MariaDB, TiDB, SQLite, MongoDB, Redis, Elasticsearch, or ClickHouse databases.
---

# WhoDB Database Assistant

You have access to WhoDB for database operations. Use these tools and commands to help users with database tasks.

## MCP Tools (Preferred)

When the WhoDB MCP server is available, use these tools directly:

### whodb_connections
List all available database connections.
```
No parameters required.
Returns: List of connection names with type and source (env/saved).
```

### whodb_query
Execute SQL queries against a database.
```
Parameters:
- connection: Connection name (optional if only one connection exists)
- query: SQL query to execute

Example: whodb_query(connection="mydb", query="SELECT * FROM users LIMIT 10")
```

### whodb_schemas
List all schemas in a database.
```
Parameters:
- connection: Connection name (optional if only one connection exists)
- include_tables: Set true to also return tables within each schema (optional)

Example: whodb_schemas(connection="mydb")
Example: whodb_schemas(connection="mydb", i
```

</details>
