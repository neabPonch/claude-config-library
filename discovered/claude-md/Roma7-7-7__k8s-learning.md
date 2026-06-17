---
name: Roma7-7-7__k8s-learning
source: https://github.com/Roma7-7-7/k8s-learning/blob/68b7c6be9ab4bb1d41b84370b2b11e5140ddd6a4/claude.md
repo: Roma7-7-7/k8s-learning
kind: claude-md
stars: 0
last_pushed: 2025-10-29T09:53:16Z
license: mit
score: 8
domains: [backend, devops, kubernetes]
tags: [go, k8s, infrastructure]
curated: 2026-06-16
curated_by: config-scout
---

# Roma7-7-7/k8s-learning — claude-md

**Why it's worth keeping:** Includes specific implementation details for health endpoints, error wrapping patterns, and K8s controller best practices like using Patch over Update.

**Summary:** Comprehensive guidelines for Go development and Kubernetes orchestration, focusing on production-ready standards.

**Source credibility:** Low star count/unproven source, but the technical depth suggests a professional engineer's standards.

**Recency:** Current; utilizes modern Go toolsets (slog) and standard Kubernetes observability patterns.

**Source:** [Roma7-7-7/k8s-learning/claude.md](https://github.com/Roma7-7-7/k8s-learning/blob/68b7c6be9ab4bb1d41b84370b2b11e5140ddd6a4/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project Guidelines for Claude Code

## Go Coding Standards

### Code Style
- Follow standard Go conventions and use `gofmt` formatting
- Use meaningful variable and function names
- Prefer short, descriptive names for local variables
- Use PascalCase for exported functions/types, camelCase for unexported
- Keep functions small and focused on a single responsibility
- Don't add package name to struct name (e.g., `User` instead of `UserModel` or `ModelUser` if part of `model` package)
- Run `make lint` before committing to ensure code quality and consistency
- Use `golangci-lint` for comprehensive code analysis and style checking
- Use `log` instead of `logger` to define logger struct field, arguments and parameters

### Error Handling
- Always handle errors explicitly - never ignore them
- Use wrapped errors with `fmt.Errorf("operation: %w", err)` for context
- Do not use `fmt.Errorf("failed to do something: %v", err)` - prefer simple `fmt.Errorf("to do something: %w", err)`
- Return errors as the last return value
- Prefer custom error types for domain-specific errors
- Use `errors.Is` and `errors.As` for error checking

### Dependencies
- Prefer standard library when possible
-
```

</details>
