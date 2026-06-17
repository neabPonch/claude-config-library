---
name: rapidcoderx__mcp-monorepo
source: https://github.com/rapidcoderx/mcp-monorepo/blob/6a2df639b2cc57cd0f8a9d1b29674a95f1006c9b/claude.md
repo: rapidcoderx/mcp-monorepo
kind: claude-md
stars: 0
last_pushed: 2026-02-18T03:56:28Z
license: unknown
score: 9
domains: [agents-ai, backend-api, cli-tools]
tags: [mcp, node-js, architecture-patterns, server-implementation]
curated: 2026-06-14
curated_by: config-scout
---

# rapidcoderx/mcp-monorepo — claude-md

**Why it's worth keeping:** The 'Anti-Patterns' section provides highly specific code-level instructions that prevent common SDK errors, such as improper schema usage and incorrect object initialization orders.

**Summary:** Provides rigorous architectural and implementation standards for building MCP servers with dual transport (stdio/HTTP) support.

**Source credibility:** Low social proof via star count, but the technical depth of the documentation suggests a high-quality internal framework.

**Recency:** Highly relevant; focuses on the modern Model Context Protocol (MCP) ecosystem.

**Source:** [rapidcoderx/mcp-monorepo/claude.md](https://github.com/rapidcoderx/mcp-monorepo/blob/6a2df639b2cc57cd0f8a9d1b29674a95f1006c9b/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Review Guide

## Project Overview

**MCP Monorepo Framework** - A monorepo framework for building reusable MCP (Model Context Protocol) servers with dual transport support (stdio and HTTP).

**Tech Stack:**
- **Backend**: Node.js (ESM), @modelcontextprotocol/sdk v1.26.0
- **Frontend**: React 19.2.4 + Vite 7.3.1
- **Server**: Express 4.21.2
- **Language**: Plain JavaScript with JSDoc documentation
- **Package Manager**: npm workspaces
- **Code Style**: ESLint 10 + Prettier 3.8.1

---

## Code Review Checklist

### 1. Architecture & Design

- [ ] **Dual Transport Pattern**: Does the server support both stdio and HTTP transports?
- [ ] **BaseMCPServer Extension**: Does the implementation extend `BaseMCPServer` from `@mcp/core`?
- [ ] **Independent Deployment**: Can the component be deployed standalone?
- [ ] **Proper Separation**: Is business logic separated from transport layer?

### 2. Code Quality

- [ ] **ESM Compliance**: Uses `import`/`export` (not `require`)
- [ ] **JSDoc Documentation**: All public functions have proper JSDoc comments
- [ ] **Error Handling**: Errors are caught and formatted using `formatError` middleware
- [ ] **Type Safety**: JSDoc types are ac
```

</details>
