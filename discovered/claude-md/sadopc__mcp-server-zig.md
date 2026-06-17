---
name: sadopc__mcp-server-zig
source: https://github.com/sadopc/mcp-server-zig/blob/3e5c95ace47304ef1921f94d89193e790481e874/CLAUDE.md
repo: sadopc/mcp-server-zig
kind: claude-md
stars: 2
last_pushed: 2026-02-09T12:35:45Z
license: mit
score: 9
domains: [cli-tools, language-intelligence]
tags: [zig, mcp, lsp, typescript]
curated: 2026-06-16
curated_by: config-scout
---

# sadopc/mcp-server-zig — claude-md

**Why it's worth keeping:** It documents critical implementation patterns like lazy subprocess initialization, error-wrapping strategies to prevent host crashes, and low-level dependency conflict workarounds.

**Summary:** A highly technical guide for an MCP server that bridges Claude to Zig language intelligence via ZLS/LSP. It details the system architecture, available tools, and specific runtime behaviors.

**Source credibility:** Niche specialized tool with high-quality technical documentation despite low star count.

**Recency:** Current; aligns with modern MCP SDK and LSP standards.

**Source:** [sadopc/mcp-server-zig/CLAUDE.md](https://github.com/sadopc/mcp-server-zig/blob/3e5c95ace47304ef1921f94d89193e790481e874/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

MCP server exposing Zig language intelligence (via ZLS) as 8 tools for Claude Code. TypeScript, no framework beyond the MCP SDK.

## Build & Run

```bash
pnpm install           # Install dependencies
pnpm build             # Compile TypeScript → build/
pnpm start             # Run the server (stdio transport)
pnpm dev               # Watch mode (recompile on change)
```

Requires `zig` and `zls` on PATH for tools to work. The server itself starts without them — errors surface per-tool.

## Architecture

```
Claude Code ←(MCP/stdio)→ index.ts ←(LSP/stdio)→ ZLS subprocess
                                    ←(execSync)→  zig fmt / zig build
```

- **`src/index.ts`** — Entry point. Creates `McpServer`, registers all 8 tools with zod schemas, connects `StdioServerTransport`. All tool handlers follow the same pattern: call the tool function, return `{ content: [{ type: "text", text }] }`, catch errors and return `isError: true`.
- **`src/zls-client.ts`** — `ZlsClient` class. Manages ZLS subprocess lifecycle: lazy start on first use, LSP initialize handshake, document open/close/re-sync, diagnostics collection via `textDocument/publishDiagnostics` notification, auto-restart
```

</details>
