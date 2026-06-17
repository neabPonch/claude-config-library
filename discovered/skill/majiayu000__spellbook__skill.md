---
name: majiayu000__spellbook__skill
source: https://github.com/majiayu000/spellbook/blob/e7d2beb070454aeace477fd48661d833b37c483e/skills/golang-web/SKILL.md
repo: majiayu000/spellbook
kind: skill
stars: 211
last_pushed: 2026-06-13T19:40:45Z
license: mit
score: 8
domains: [backend-api, golang]
tags: [go, architecture, boilerplate]
curated: 2026-06-16
curated_by: config-scout
---

# majiayu000/spellbook — skill

**Why it's worth keeping:** The 'no backwards compatibility' rule prevents code rot during agent-led refactors, and it provides highly specific patterns for error wrapping and dependency injection.

**Summary:** A comprehensive architectural blueprint for Go web applications using the cmd/internal/pkg pattern.

**Source credibility:** Strong; part of a specialized 'spellbook' with active maintenance and community interest.

**Recency:** Current; includes modern integrations like LiteLLM which is highly relevant for current AI-driven workflows.

**Source:** [majiayu000/spellbook/skills/golang-web/SKILL.md](https://github.com/majiayu000/spellbook/blob/e7d2beb070454aeace477fd48661d833b37c483e/skills/golang-web/SKILL.md) · 211★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: golang-web
description: Modern Go Web application architecture guide. Use when creating new Go web projects, APIs, or microservices. Covers project structure, tech stack selection, and best practices based on Go standards.
---
# Go Web Architecture

## Core Principles

- **Standard layout** — Follow cmd/internal/pkg convention
- **Explicit dependencies** — Wire dependencies in main.go, no globals
- **Interface-driven** — Define interfaces where you use them, not where you implement
- **Error wrapping** — Wrap errors with context, use error codes
- **No backwards compatibility** — Delete, don't deprecate. Change directly
- **LiteLLM for LLM APIs** — Use LiteLLM proxy for all LLM integrations

---

## No Backwards Compatibility

> **Delete unused code. Change directly. No compatibility layers.**

```go
// ❌ BAD: Deprecated function kept around
// Deprecated: Use NewUserService instead
func CreateUserService() *UserService { ... }

// ❌ BAD: Alias for renamed types
type OldName = NewName // "for backwards compatibility"

// ❌ BAD: Unused parameters
func Process(_ context.Context, data Data) { ... }

// ✅ GOOD: Just delete and update all usages
func NewUserService(repo UserRe
```

</details>
