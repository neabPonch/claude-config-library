---
name: Type-MCP__mcp-anything
source: https://github.com/Type-MCP/mcp-anything/blob/e25e491843e62861802be9601b6e3e80e25a44b5/CLAUDE.md
repo: Type-MCP/mcp-anything
kind: claude-md
stars: 37
last_pushed: 2026-05-09T18:45:35Z
license: apache-2.0
score: 9
domains: [agents-ai, mcp, codegen]
tags: [mcp, code-generation, architectural-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# Type-MCP/mcp-anything — claude-md

**Why it's worth keeping:** Provides highly opinionated '2026 Stack Defaults' (e.g., Group CRUD logic and progressive disclosure) that are perfect-in-a-row instructions for an AI to maintain architectural consistency.

**Summary:** A technical blueprint defining a multi-phase pipeline for generating optimized MCP servers via domain modeling and code emission.

**Source credibility:** High-quality, specialized technical documentation from an active MCP automation repository.

**Recency:** Extremely current, featuring 2026-dated verification and recent bug-fix history.

**Source:** [Type-MCP/mcp-anything/CLAUDE.md](https://github.com/Type-MCP/mcp-anything/blob/e25e491843e62861802be9601b6e3e80e25a44b5/CLAUDE.md) · 37★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# MCP-Anything

## What this project does
LLM-driven pipeline that takes a customer's domain brief (use-cases in natural language)
and a data source (OpenAPI / gRPC / DB schema / SDK), and produces a fully-implemented,
optimized MCP server plus skill bundle and validation artifacts.

Three output backends: **Python/FastMCP**, **TypeScript/mcp-use**, and **TypeScript/Skybridge** (MCP + ChatGPT App with React views).

Legacy path: `mcp-anything generate <path>` (codebase scanner, backwards-compatible).
Domain path: `mcp-anything build --brief <brief.yaml>` (new, recommended).

## Development
- Install: `pip install -e ".[dev,llm]"`
- Run tests: `pytest tests/ -v`
- Run CLI: `mcp-anything --help`

## Architecture

### Domain Pipeline (new, primary)
5 phases: DOMAIN_MODELING → TOOL_DESIGN → EMIT → SKILL_BUNDLE → VALIDATION_HARNESS
- Phase 1 (`domain_modeling.py`): LLM reads brief + data source → `domain_model.json`
- Phase 2 (`tool_design.py`): LLM shapes tools per 2026 rules → `tool_spec.yaml`
- Phase 3 (`emit/python_fastmcp/`, `emit/typescript_mcp_use/`, or `emit/typescript_skybridge/`): code generation
- Phase 4 (`skill_bundle.py`): LLM generates `SKILL.md` + `quick_queries.json`
-
```

</details>
