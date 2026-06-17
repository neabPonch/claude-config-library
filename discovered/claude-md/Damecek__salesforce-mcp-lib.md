---
name: Damecek__salesforce-mcp-lib
source: https://github.com/Damecek/salesforce-mcp-lib/blob/66574f921a9af571bc52a54b064df5deef464fdb/CLAUDE.md
repo: Damecek/salesforce-mcp-lib
kind: claude-md
stars: 15
last_pushed: 2026-04-14T10:22:53Z
license: mit
score: 8
domains: [cli-tools, cloud-integration, security]
tags: [nodejs, typescript, salesforce, mcp, devops]
curated: 2026-06-15
curated_by: config-scout
---

# Damecek/salesforce-mcp-lib — claude-md

**Why it's worth keeping:** The 'Active Technologies' section prevents dependency bloat by forbidding npm packages, while the explicit git tag format eliminates ambiguity in multi-part versioning.

**Summary:** Establishes strict architectural constraints regarding zero-dependency Node.js usage and provides a highly specific dual-package release/tagging protocol.

**Source credibility:** Highly specialized technical content suggesting professional development standards for a niche toolset.

**Recency:** Very current; utilizes modern Node.js and includes future-dated/highly recent maintenance logs.

**Source:** [Damecek/salesforce-mcp-lib/CLAUDE.md](https://github.com/Damecek/salesforce-mcp-lib/blob/66574f921a9af571bc52a54b064df5deef464fdb/CLAUDE.md) · 15★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# salesforce-mcp-lib Development Guidelines

Auto-generated from all feature plans. Last updated: 2026-04-08

## Active Technologies
- TypeScript ES2022, Node.js >= 20.0.0 + Zero production dependencies. Node.js built-in modules only (`node:http`, `node:https`, `node:fs`, `node:path`, `node:crypto`, `node:os`, `node:child_process`, `node:readline`, `node:url`) (003-per-user-auth)
- File-based token persistence in `~/.salesforce-mcp-lib/tokens/` (0600 permissions) (003-per-user-auth)

- Apex (Salesforce API 65.0) + TypeScript (ES2022, Node.js >= 20) + Zero external dependencies. Apex uses platform-native APIs only. TypeScript uses Node.js built-in modules only (no production npm dependencies). JSON-RPC 2.0 core is implemented in-repo, not imported. (001-apex-mcp-server)

## Project Structure

```text
packages/salesforce-mcp-lib/src/
  index.ts             # CLI entry point (login subcommand + MCP server)
  config.ts            # CLI argument / env-var parser
  types.ts             # Shared type definitions (AuthConfig, AuthMode, etc.)
  errors.ts            # Error class hierarchy (SalesforceAuthError + subclasses)
  oauth.ts             # Client credentials OAuth flow + ClientCrede
```

</details>
