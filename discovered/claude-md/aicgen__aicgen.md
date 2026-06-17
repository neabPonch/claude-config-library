---
name: aicgen__aicgen
source: https://github.com/aicgen/aicgen/blob/a0d77c3f11105c0730544827c1d23c1d4088e783/claude.md
repo: aicgen/aicgen
kind: claude-md
stars: 3
last_pushed: 2026-05-26T15:11:29Z
license: mit
score: 8
domains: [software-engineering, ai-agents, devops]
tags: [modular, sdlc, workflow-automation]
curated: 2026-06-14
curated_by: config-scout
---

# aicgen/aicgen — claude-md

**Why it's worth keeping:** The pattern of delegating specific domains to sub-files (@.claude/...) prevents file bloat, and the phase-based workflow (/spec -> /ship) provides a clear execution framework for agentic tasks.

**Summary:** A meta-template that implements a highly modularized documentation structure and a rigorous SDLC via custom slash commands.

**Source credibility:** Low; it is an auto-generated sample from a configuration generator tool.

**Recency:** Current; aligns with advanced agentic capabilities like subagents and skill-based profiles.

**Source:** [aicgen/aicgen/claude.md](https://github.com/aicgen/aicgen/blob/a0d77c3f11105c0730544827c1d23c1d4088e783/claude.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# my-project - Development Guidelines

**Role:** You are an expert software engineer specialized in typescript and layered architecture.
**User's Goal:** Build high-quality, maintainable software following strict project guidelines.

## Guidelines

This project follows structured coding guidelines organized by category:

- **Language**: @.claude/guidelines/language.md
- **Architecture**: @.claude/guidelines/architecture.md
- **Testing**: @.claude/guidelines/testing.md
- **Security**: @.claude/guidelines/security.md
- **Performance**: @.claude/guidelines/performance.md
- **API Design**: @.claude/guidelines/api-design.md
- **Code Style**: @.claude/guidelines/code-style.md
- **Error Handling**: @.claude/guidelines/error-handling.md
- **DevOps**: @.claude/guidelines/devops.md
- **Best Practices**: @.claude/guidelines/best-practices.md
- **Design Patterns**: @.claude/guidelines/design-patterns.md

## Quick Reference

- Run tests: Check package.json scripts
- Build: Check package.json scripts
- Code style: See Code Style guidelines above
- Architecture: See Architecture guidelines above

## Workflows

Use these slash commands for structured SDLC delivery:

Flow: `/spec` → `/research` → `
```

</details>
