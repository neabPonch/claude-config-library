---
name: wadearnold__idiomatic-go-claude-template
source: https://github.com/wadearnold/idiomatic-go-claude-template/blob/1d63a9a5eb5bbc744dd15faa97d9ef476a5a15c7/claude.md
repo: wadearnold/idiomatic-go-claude-template
kind: claude-md
stars: 10
last_pushed: 2025-07-18T17:23:05Z
license: apache-2.0
score: 8
domains: [backend, cli-tools]
tags: [modular-docs, quality-assurance, go]
curated: 2026-06-16
curated_by: config-scout
---

# wadearnold/idiomatic-go-claude-template — claude-md

**Why it's worth keeping:** The 'modular context' pattern (using sub-docs) prevents CLAUDE.md bloat; the explicit 'Quality Gates' provide high-signal guardrails for AI-driven commits.

**Summary:** Establishes a modular documentation system by directing Claude to specific guidelines within a hidden .claude/ directory and defines strict quality gates.

**Source credibility:** Small repository but demonstrates a professional, high-standard approach to Go development.

**Recency:** 

**Source:** [wadearnold/idiomatic-go-claude-template/claude.md](https://github.com/wadearnold/idiomatic-go-claude-template/blob/1d63a9a5eb5bbc744dd15faa97d9ef476a5a15c7/claude.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Go Development Context

This project follows strict Go development standards. All code must be idiomatic, well-tested, and properly formatted.

## File Organization
All Claude-related files are organized in the `.claude/` directory to keep the project root clean.

## Style Guidelines
See [Go Style Guidelines](./.claude/docs/go-style.md) for detailed coding standards.

## Commit Standards  
See [Commit Standards](./.claude/docs/commit-standards.md) for pre-commit requirements.

## Project Organization
See [Project Organization](./.claude/docs/project-organization.md) for directory structure rules.

## Quick Reference

### Before Every Commit
```bash
make commit-ready  # Must pass before git commit
```

### Code Style Priorities
1. Follow Effective Go and standard library patterns
2. Prefer concrete types over interfaces
3. Avoid package name stuttering
4. Use short, meaningful names
5. Zero tolerance for formatting violations

### Quality Gates
- All linters must pass (golangci-lint, gitleaks, govulncheck)
- Test coverage ≥ 85%
- All tests pass with race detection
- Clean builds with no warnings

### Project Organization Rules
- Keep project root clean - no scripts, docs, or binar
```

</details>
