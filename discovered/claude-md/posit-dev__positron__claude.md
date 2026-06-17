---
name: posit-dev__positron__claude
source: https://github.com/posit-dev/positron/blob/2e4cbb5c3ec54f0467df91d13a1fd8e5ba9f0233/extensions/positron-duckdb/CLAUDE.md
repo: posit-dev/positron
kind: claude-md
stars: 4163
last_pushed: 2026-06-15T07:28:11Z
license: other
score: 9
domains: [extension-development, data-science-tools, node-js]
tags: [duckdb, typescript, rpc, native-bindings]
curated: 2026-06-15
curated_by: config-scout
---

# posit-dev/positron — claude-md

**Why it's worth keeping:** Includes specific 'Do Not' warnings for auto-generated files, exact CLI command patterns for testing/daemons, and clear mapping of data types to display types.

**Summary:** Provides deep technical context for a specialized DuckDB extension, covering internal architecture, RPC protocol integration, and developer workflows.

**Source credibility:** High; part of the high-star Positron repository maintained by a professional team.

**Recency:** Highly current based on very recent commit history.

**Source:** [posit-dev/positron/extensions/positron-duckdb/CLAUDE.md](https://github.com/posit-dev/positron/blob/2e4cbb5c3ec54f0467df91d13a1fd8e5ba9f0233/extensions/positron-duckdb/CLAUDE.md) · 4163★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Positron DuckDB Extension Development Context

This prompt provides context for working with the `positron-duckdb` extension, which provides native DuckDB support for headless data exploration in Positron.

**Related documentation:**
- **Build system**: `.claude/build-system.md` - For daemon management and compilation
- **Data Explorer UI**: `.claude/data-explorer.md` - For frontend components that use this extension
- **Testing**: `.claude/e2e-testing.md` - For E2E tests involving data exploration

## Extension Overview

**Purpose**: Provides DuckDB support for headless data explorers for previewing data files  
**Display Name**: "Positron DuckDB Support"  
**Location**: `extensions/positron-duckdb/`  
**Main Entry**: `src/extension.ts`  
**Dependencies**: `@duckdb/node-api` (pulls in the platform-specific `@duckdb/node-bindings-*` native binding for the host)  

The extension uses the native `@duckdb/node-api` ("node neo") package, which wraps pre-built DuckDB binaries. It reads compressed CSV/TSV files and supports multithreading.

## Architecture

### Core Components

1. **DuckDBInstance**: Manages the native DuckDB database connection (`@duckdb/node-api`)
2. **QueryResult**:
```

</details>
