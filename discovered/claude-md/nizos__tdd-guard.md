---
name: nizos__tdd-guard
source: https://github.com/nizos/tdd-guard/blob/73b647f8c4ac43753d61d1063f12b0fab527f050/CLAUDE.md
repo: nizos/tdd-guard
kind: claude-md
stars: 2196
last_pushed: 2026-06-08T14:05:43Z
license: mit
score: 8
domains: [cli-tools, tdd, typescript]
tags: [tdd, engineering-standards, testing-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# nizos/tdd-guard — claude-md

**Why it's worth keeping:** The prescriptive commit message format (explaining 'why' vs 'what') and the specific requirements for test implementation (using factories/helpers) provide perfect constraints for an AI agent.

**Summary:** Provides highly structured engineering standards for a TDD-focused workflow, covering commits, testing patterns, and architecture.

**Source credibility:** High; 2k+ stars and active maintenance indicate a widely used tool.

**Recency:** Extremely current; explicitly mentions Claude Code integration and recent updates.

**Source:** [nizos/tdd-guard/CLAUDE.md](https://github.com/nizos/tdd-guard/blob/73b647f8c4ac43753d61d1063f12b0fab527f050/CLAUDE.md) · 2196★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# TDD Guard

## Project Goal

TDD Guard is a Claude Code hook that enforces Test-Driven Development by intercepting file operations.
When Claude Code attempts to edit or write files, TDD Guard:

1. **Captures**: Intercepts Edit, MultiEdit, and Write operations
2. **Analyzes**: Examines test results, file paths, and code changes
3. **Validates**: Checks TDD compliance using an AI model
4. **Blocks**: Prevents operations that skip tests or over-implement
5. **Guides**: Explains violations and suggests corrections

This automated enforcement maintains code quality without cluttering prompts with TDD reminders.

## Development Workflow

### Commit Guidelines

- **Atomic commits**: Each commit represents one logical change with its tests
- **Test and implementation together**: Never separate tests from the code they test
- **Explain why, not what**: Commit messages should explain the reason for the change
- **Conventional format**: Use prefixes to categorize changes: feat, fix, refactor, test, chore, docs

Example: `feat: add network request filtering to reduce noise in captured data` (explains why, not just what)

## Project Structure

The codebase is organized with core functionality
```

</details>
