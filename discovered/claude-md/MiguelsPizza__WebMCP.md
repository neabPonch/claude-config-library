---
name: MiguelsPizza__WebMCP
source: https://github.com/MiguelsPizza/WebMCP/blob/1143b2184edd4f33ef60fd1d10b0d71c26a2e87e/CLAUDE.md
repo: MiguelsPizza/WebMCP
kind: claude-md
stars: 1070
last_pushed: 2025-10-07T18:19:45Z
license: other
score: 9
domains: [browser-extensions, monorepo, mcp-protocol, web-development]
tags: [monorepo, architecture-first, pnpm, extension-dev]
curated: 2026-06-14
curated_by: config-scout
---

# MiguelsPizza/WebMCP — claude-md

**Why it's worth keeping:** It explains the 'why' behind its architecture (Traditional vs. MCP-B), which prevents AI from making wrong design assumptions; it also uses granular pnpm filters perfect for agentic task execution in monorepos.

**Summary:** A comprehensive guide that combines essential command lists with a deep architectural mental model for an MCP-based monorepo.

**Source credibility:** High credibility with 1k+ stars and a well-defined technical stack.

**Recency:** 

**Source:** [MiguelsPizza/WebMCP/CLAUDE.md](https://github.com/MiguelsPizza/WebMCP/blob/1143b2184edd4f33ef60fd1d10b0d71c26a2e87e/CLAUDE.md) · 1070★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Prerequisites
- Node.js >=22.12 (recommended: 24.3.0 per .nvmrc)
- pnpm ^10
- Chrome browser for extension development

## Essential Commands

### Development Setup
- `pnpm install` - Install all dependencies across the monorepo
- `pnpm build:shared` - Build all shared internal packages
- `pnpm build:apps` - Build all applications (extension, backend, native-server)
- `pnpm dev` - Start all development servers with automatic native messaging registration
- `pnpm dev:apps` - Start development servers for all apps
- `pnpm dev:mcp` - Start only extension and native-server (useful for MCP development)

### Build and Quality
- `pnpm build` - Build all projects in the monorepo (runs build:packages first, then builds apps)
- `pnpm typecheck` - Type-check all TypeScript files across the workspace
- `pnpm lint` - Run Biome linter with auto-fix
- `pnpm format` - Format code with Biome
- `pnpm check` - Run both linting and formatting checks
- `pnpm check-all` - Complete quality check (typecheck + biome ci)

### Testing
- `pnpm test` - Run all tests across the monorepo with T
```

</details>
