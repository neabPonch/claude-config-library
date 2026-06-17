---
name: timescale__pg-aiguide
source: https://github.com/timescale/pg-aiguide/blob/a542650e4c87b619ac4ee0174f536a02860bf9e8/CLAUDE.md
repo: timescale/pg-aiguide
kind: claude-md
stars: 1762
last_pushed: 2026-06-10T15:10:07Z
license: apache-2.0
score: 8
domains: [mcp-servers, cli-tools, backend-api]
tags: [bun, typescript, mcp, tool-calling]
curated: 2026-06-14
curated_by: config-scout
---

# timescale/pg-aiguide — claude-md

**Why it's worth keeping:** Includes a high-value specific instruction to use '.nullable()' instead of '.optional()' for tool parameters to optimize LLM compatibility. It also provides exact CLI workflows for building, watching, and running the server via stdio.

**Summary:** Provides essential build commands and strict coding standards tailored for developing MCP servers using TypeScript and Bun.

**Source credibility:** High; maintained by Timescale with recent activity and significant community interest (1700+ stars).

**Recency:** Current; utilizes modern tooling (Bun) and addresses specific nuances of contemporary LLM tool-calling requirements.

**Source:** [timescale/pg-aiguide/CLAUDE.md](https://github.com/timescale/pg-aiguide/blob/a542650e4c87b619ac4ee0174f536a02860bf9e8/CLAUDE.md) · 1762★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Tiger Docs MCP Server - Development Guidelines

## Build, Test & Run Commands

- Build: `./bun run build` - Compiles TypeScript to JavaScript
- Watch mode: `./bun run watch http` - Watches for changes and rebuilds automatically
- Run server: `./bun run start stdio` - Starts the MCP server using stdio transport
- Checks: `./bun run check` - All-in-one command to lint and test. Run before every commit.

## Code Style Guidelines

- Use ES modules with `.js` extension in import paths
- Strictly type all functions and variables with TypeScript
- Follow zod schema patterns for tool input validation
- Use `.nullable()` instead of `.optional()` for optional MCP tool parameters (required for gpt-5 compatibility)
- Prefer async/await over callbacks and Promise chains
- Place all imports at top of file, grouped by external then internal
- Use descriptive variable names that clearly indicate purpose
- Implement proper cleanup for timers and resources in server shutdown
- Follow camelCase for variables/functions, PascalCase for types/classes, UPPER_CASE for constants
- Handle errors with try/catch blocks and provide clear error messages
- Use consistent indentation (2 spaces) and trailing com
```

</details>
