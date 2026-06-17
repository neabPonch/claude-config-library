---
name: apache__skywalking-mcp
source: https://github.com/apache/skywalking-mcp/blob/06e2b6413f7b592770b6c5c62b28144f88382b49/CLAUDE.md
repo: apache/skywalking-mcp
kind: claude-md
stars: 27
last_pushed: 2026-04-02T02:10:45Z
license: apache-2.0
score: 9
domains: [cli-tools, backend-api, observability]
tags: [mcp, go, architecture-guide, extensibility]
curated: 2026-06-14
curated_by: config-scout
---

# apache/skywalking-mcp — claude-md

**Why it's worth keeping:** The 'Extending the Server' section provides actionable recipes for new features, while the architecture/validation sections prevent AI from hallucinating invalid system behaviors.

**Summary:** An excellent technical blueprint that bridges the gap between high-level overview and low-level implementation details.

**Source credibility:** High; maintained by an Apache Software Foundation project with established engineering standards.

**Recency:** Current; specifically tailored to modern MCP (Model Context Protocol) development patterns.

**Source:** [apache/skywalking-mcp/CLAUDE.md](https://github.com/apache/skywalking-mcp/blob/06e2b6413f7b592770b6c5c62b28144f88382b49/CLAUDE.md) · 27★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - AI Assistant Guide for Apache SkyWalking MCP

This file provides guidance for AI assistants working with the Apache SkyWalking MCP codebase.

## Project Overview

Apache SkyWalking MCP — an MCP (Model Context Protocol) server that bridges AI agents with Apache SkyWalking OAP via GraphQL. It exposes SkyWalking's observability data (traces, logs, metrics, topology, alarms, events) as MCP tools, prompts, and resources. Binary name: `swmcp`.

## Repository Structure

```
skywalking-mcp/
├── cmd/skywalking-mcp/       # Entry point (cobra/viper CLI, three subcommands)
├── internal/
│   ├── config/               # Config structs for each transport mode
│   ├── swmcp/                # MCP server factory + transport adapters (stdio/sse/streamable)
│   ├── tools/                # MCP tool implementations (16 tools, grouped by domain)
│   ├── prompts/              # MCP prompt definitions (10 prompts, three groups)
│   └── resources/            # MCP resources (embedded MQE docs + dynamic metrics)
└── dist/                     # Distribution license files
```

## Build & Development Commands

```bash
make build            # Build binary to bin/swmcp
make lint             # Run g
```

</details>
