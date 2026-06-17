---
name: petems__hardcover-cli
source: https://github.com/petems/hardcover-cli/blob/6b1eee2f54684f4787bf64462d4006309768b98a/CLAUDE.MD
repo: petems/hardcover-cli
kind: claude-md
stars: 1
last_pushed: 2026-02-16T09:16:10Z
license: mit
score: 9
domains: [cli-tools, backend-api, golang]
tags: [pattern-matching, structural-guidance, test-driven]
curated: 2026-06-16
curated_by: config-scout
---

# petems/hardcover-cli — claude-md

**Why it's worth keeping:** The 'Common Tasks' section uses concrete code snippets to define structural patterns (e.g., Cobra command setup), which is the most effective way to enforce consistency in AI generation.

**Summary:** Provides a high-density map of project structure, specific implementation patterns, and technical limitations.

**Source credibility:** Single-star repository, but the file quality suggests a highly organized developer using LLM-driven workflows.

**Recency:** Current; uses modern Go 1.23+ context and follows contemporary Claude Code prompting best practices.

**Source:** [petems/hardcover-cli/CLAUDE.MD](https://github.com/petems/hardcover-cli/blob/6b1eee2f54684f4787bf64462d4006309768b98a/CLAUDE.MD) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude AI Configuration for Hardcover CLI

## Project Context

This is a Go-based CLI application for interacting with the Hardcover.app GraphQL API. The project follows modern Go development practices with comprehensive testing and documentation.

## Key Information for Claude

### Project Structure
- **Language**: Go 1.23+
- **Framework**: Cobra CLI framework
- **API**: GraphQL with Hardcover.app
- **Testing**: Testify framework with high coverage
- **Configuration**: YAML files and environment variables

### Current State
- ✅ User profile management (`hardcover me`)
- ✅ Book search (`hardcover search books <query>`)
- ✅ User search (`hardcover search users <query>`)
- ✅ Configuration management (`hardcover config`)
- ⚠️ Limited to read-only operations
- ⚠️ Some API schema inconsistencies

### Important Files
- `cmd/root.go` - Main CLI setup and command registration
- `cmd/search.go` - Search functionality implementation
- `cmd/me.go` - User profile commands
- `cmd/config.go` - Configuration management
- `internal/client/client.go` - GraphQL client
- `internal/config/config.go` - Configuration logic
- `internal/client/schema.graphql` - GraphQL schema
- `internal/client/queries.
```

</details>
