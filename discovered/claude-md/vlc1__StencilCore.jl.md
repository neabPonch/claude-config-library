---
name: vlc1__StencilCore.jl
source: https://github.com/vlc1/StencilCore.jl/blob/81db3bf70d909eb0ea726bf004bee2302d35f80b/CLAUDE.md
repo: vlc1/StencilCore.jl
kind: claude-md
stars: 0
last_pushed: 2026-06-01T10:56:55Z
license: unknown
score: 7
domains: [scientific-computing, cli-tools]
tags: [mcp, julia, environment-setup]
curated: 2026-06-16
curated_by: config-scout
---

# vlc1/StencilCore.jl — claude-md

**Why it's worth keeping:** Includes specific command-line sequences to troubleshoot MCP tool availability, which is a critical failure point when using specialized language servers.

**Summary:** Provides explicit setup and verification steps for integrating the julia-mcp server into the Claude Code environment.

**Source credibility:** Low visibility (0 stars); likely a niche or academic scientific computing project.

**Recency:** Current; utilizes modern Claude Code 'mcp' CLI commands.

**Source:** [vlc1/StencilCore.jl/CLAUDE.md](https://github.com/vlc1/StencilCore.jl/blob/81db3bf70d909eb0ea726bf004bee2302d35f80b/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

@./AGENTS.md

## MCP Servers

This project uses the [julia-mcp](https://github.com/aplavin/julia-mcp) MCP server
for Julia language tooling. Before starting any work, verify it is active:

```bash
claude mcp list
```

If `julia-mcp` is not listed or shows as disconnected, add it:

```bash
claude mcp add --transport stdio julia-mcp -- <command-from-julia-mcp-readme>
```

Then use `/mcp` inside the session to confirm the tools are available before proceeding.
```

</details>
