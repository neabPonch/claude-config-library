---
name: apache__dubbo-go-pixiu__skill
source: https://github.com/apache/dubbo-go-pixiu/blob/331735d3cfd1dd2170ad53f5c11f845fc34035e6/skills/pixiu-mcp-integration/SKILL.md
repo: apache/dubbo-go-pixiu
kind: skill
stars: 554
last_pushed: 2026-06-14T05:53:40Z
license: apache-2.0
score: 9
domains: [ai-gateway, backend-infrastructure, security]
tags: [mcp, api-gateway, dubbo-go, protocol-mapping]
curated: 2026-06-16
curated_by: config-scout
---

# apache/dubbo-go-pixiu — skill

**Why it's worth keeping:** It uses a 'Step 0' source-verification pattern that forces the agent to check actual code before generating config; it also includes exact filter ordering and precise curl commands for smoke testing.

**Summary:** A highly structured technical guide for configuring Pixiu as an MCP gateway via HTTP/SSE, including authentication sequencing and dynamic tool discovery.

**Source credibility:** High; comes from an active Apache Dubbo-Go repository with recent commits.

**Recency:** Very current; specifically addresses modern Model Context Protocol (MCP) standards.

**Source:** [apache/dubbo-go-pixiu/skills/pixiu-mcp-integration/SKILL.md](https://github.com/apache/dubbo-go-pixiu/blob/331735d3cfd1dd2170ad53f5c11f845fc34035e6/skills/pixiu-mcp-integration/SKILL.md) · 554★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pixiu-mcp-integration
description: |
  Use when configuring dubbo-go-pixiu as an MCP gateway:
  `dgp.filter.mcp.mcpserver`, Streamable HTTP/SSE, `tools/list`,
  `tools/call`, OAuth/JWT `dgp.filter.http.auth.mcp`, Nacos
  `dgp.adapter.mcpserver`, or stdio MCP bridge guidance.
allowed-tools: [Read, Grep, Glob, Edit, Write, Bash]
metadata:
  version: "0.1.1"
  domain: ai-gateway
  scope: generate-and-validate
  triggers: ["MCP", "Model Context Protocol", "mcpserver", "tools/list", "tools/call", "Mcp-Session-Id", "dgp.filter.mcp.mcpserver", "dgp.filter.http.auth.mcp", "mcp gateway", "MCP tool"]
  pixiu_min_version: "0.6.0"
  experimental: true
  role: specialist
---

# pixiu-mcp-integration — Exposing HTTP APIs as MCP Tools

Pixiu's current MCP integration is an HTTP filter that speaks MCP
Streamable HTTP/SSE to clients and maps `tools/call` to backend HTTP
clusters. It can also expose resources, resource templates, prompts,
and optional OAuth/JWT protection.

Important boundary: current Pixiu does not directly spawn or manage
stdio MCP servers. For a stdio server, put an external bridge in front
of it, then configure Pixiu to call the bridge as an HTTP backend tool.

## When
```

</details>
