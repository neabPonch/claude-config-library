---
name: bhauman__clojure-mcp
source: https://github.com/bhauman/clojure-mcp/blob/94ff5c7bba93c739268bc8895a900038f0e9fa79/CLAUDE.md
repo: bhauman/clojure-mcp
kind: claude-md
stars: 762
last_pushed: 2026-06-13T00:35:58Z
license: epl-2.0
score: 8
domains: [cli-tools, agents-ai, backend]
tags: [clojure, mcp, tool-development]
curated: 2026-06-14
curated_by: config-scout
---

# bhauman/clojure-mcp — claude-md

**Why it's worth keeping:** The 'no backwards compatibility' rule for tool contracts is a high-value meta-instruction, and the highly specific test/lint command templates are immediately actionable.

**Summary:** Provides precise build commands for Clojure and specific architectural guidelines for developing MCP tools.

**Source credibility:** High: strong star count (762) and active maintenance indicated by recent commits.

**Recency:** Very current; includes modern prompting context like 'Fast Apply' patterns for tool use.

**Source:** [bhauman/clojure-mcp/CLAUDE.md](https://github.com/bhauman/clojure-mcp/blob/94ff5c7bba93c739268bc8895a900038f0e9fa79/CLAUDE.md) · 762★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Clojure MCP Development Guide

## Build Commands
- Run REPL with MCP server: `clojure -X:mcp` (starts on port 7888)
- Run all tests: `clojure -M:test`
- Run specific namespace tests: `clojure -M:test -n clojure-mcp.utils.valid-paths-test`
- Run specific test var: `clojure -M:test -v clojure-mcp.utils.valid-paths-test/clojure-file?-test`
- Run linter: `clj-kondo --lint src` or `clj-kondo --lint src test` for both

## Code Style Guidelines
- **Imports**: Use `:require` with ns aliases (e.g., `[clojure.string :as string]`)
- **Naming**: Use kebab-case for vars/functions; end predicates with `?` (e.g., `is-top-level-form?`)
- **Error handling**: Use `try/catch` with specific exception handling; atom for tracking errors
- **Formatting**: 2-space indentation; maintain whitespace in edited forms
- **Namespaces**: Align with directory structure (`clojure-mcp.repl-tools`)
- **Testing**: Use `deftest` with descriptive names; `testing` for subsections; `is` for assertions
- **REPL Development**: Prefer REPL-driven development for rapid iteration and feedback

## MCP Tool Guidelines
- Include clear tool `:description` for LLM guidance
- Validate inputs and provide helpful error messages
- Re
```

</details>
