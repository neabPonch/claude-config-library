---
name: AImaginationLab__vulnerable-llms
source: https://github.com/AImaginationLab/vulnerable-llms/blob/3310611c38da20a239ac133dcd1d3c5a8afa4941/CLAUDE.md
repo: AImaginationLab/vulnerable-llms
kind: claude-md
stars: 5
last_pushed: 2025-06-14T05:41:13Z
license: mit
score: 8
domains: [web-frontend, backend-api, security, devops]
tags: [fullstack, react, fastapi, docker, architectural-patterns]
curated: 2026-06-14
curated_by: config-scout
---

# AImaginationLab/vulnerable-llms — claude-md

**Why it's worth keeping:** It provides high-value 'Patterns to Replace' and specific architectural constraints (like using app.state instead of globals) that prevent an AI from introducing common anti-patterns.

**Summary:** A comprehensive guide for a full-stack application covering backend architecture, frontend component standards, and Docker orchestration.

**Source credibility:** High; a specialized security tool with deep technical documentation.

**Recency:** Slightly dated (12 months), but the technical stack and instructions remain highly relevant for modern development.

**Source:** [AImaginationLab/vulnerable-llms/CLAUDE.md](https://github.com/AImaginationLab/vulnerable-llms/blob/3310611c38da20a239ac133dcd1d3c5a8afa4941/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Development Notes

## Project Guidelines

### Logging
- **Always use logger instead of print statements** in Python backend code
- Use appropriate log levels (info, warning, error, debug)
- Example: `logger.info("message")` instead of `print("message")`

### Code Quality
- Follow existing code patterns and conventions
- Use proper error handling
- Add type hints where applicable
- Use FastAPI app.state for component management (not globals)

### Frontend Code Style
- **Prefer CSS classes over inline styles** - Use existing CSS classes from index.css
- **Reuse existing UI components** - Use Card, Alert, Button components from components/ui
- **Use semantic class names** - Like output-panel, demo-section, help-text
- **Avoid inline style objects** - Extract to CSS classes for maintainability
- **Follow component composition** - Break down complex UI into smaller components

### Frontend UI Components
- **Use ChatInterface for all LLM interactions** - Provides consistent user experience
- **EnhancedChatInterface** - Use for demos with attack levels/difficulty settings
- **Keep UI compact and clean** - Avoid clunky layouts, integrate controls elegantly
- **Consolidate related
```

</details>
