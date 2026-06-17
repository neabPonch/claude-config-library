---
name: QuantGeekDev__mcp-framework
source: https://github.com/QuantGeekDev/mcp-framework/blob/ead9c4bbcd5fd098e80ccf64758bd6bf43234f90/CLAUDE.md
repo: QuantGeekDev/mcp-framework
kind: claude-md
stars: 921
last_pushed: 2026-04-16T11:52:34Z
license: mit
score: 9
domains: [backend-api, cli-tools, security, ai-agents]
tags: [typescript, mcp, oauth, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# QuantGeekDev/mcp-framework — claude-md

**Why it's worth keeping:** Explicitly highlights mandatory Zod description requirements to prevent build failures and clarifies complex path resolution logic for node_modules-based dependencies.

**Summary:** Provides a highly detailed architectural blueprint and crucial technical constraints for an MCP framework.

**Source credibility:** High-quality repository with significant community traction (921 stars) and recent maintenance.

**Recency:** Very current, including specific 2025 OAuth 2.1 compliance details.

**Source:** [QuantGeekDev/mcp-framework/CLAUDE.md](https://github.com/QuantGeekDev/mcp-framework/blob/ead9c4bbcd5fd098e80ccf64758bd6bf43234f90/CLAUDE.md) · 921★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

mcp-framework is a TypeScript framework for building Model Context Protocol (MCP) servers. It provides an opinionated architecture with automatic directory-based discovery for tools, resources, and prompts. The framework is used as a dependency in other projects (similar to Express.js) and runs from node_modules.

## Development Commands

### Build and Watch
```bash
npm run build          # Compile TypeScript to dist/
npm run watch          # Watch mode for development
```

### Testing
```bash
npm test                    # Run all tests
npm run test:watch          # Run tests in watch mode
npm run test:coverage       # Run tests with coverage report
```

### Linting and Formatting
```bash
npm run lint            # Run ESLint
npm run lint:fix        # Run ESLint with auto-fix
npm run format          # Format code with Prettier
```

### Local Development with yalc
```bash
npm run dev:pub         # Build and publish to yalc for local testing
```

### CLI Commands (for projects using the framework)
```bash
mcp create <project-name>           # Create
```

</details>
