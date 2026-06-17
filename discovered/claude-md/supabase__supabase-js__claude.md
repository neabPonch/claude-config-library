---
name: supabase__supabase-js__claude
source: https://github.com/supabase/supabase-js/blob/a25062e9285fa8e3bd702c59ddda0d87ad1fcc27/.claude/CLAUDE.md
repo: supabase/supabase-js
kind: claude-md
stars: 4475
last_pushed: 2026-06-15T06:55:45Z
license: mit
score: 9
domains: [monorepo, javascript, tooling]
tags: [nx, typescript, testing-infrastructure]
curated: 2026-06-15
curated_by: config-scout
---

# supabase/supabase-js — claude-md

**Why it's worth keeping:** The detailed command reference table—mapping packages to Docker dependencies—is exceptionally useful for preventing failed test runs. It also establishes strict 'Zero Breaking Change' behavior as a core principle.

**Summary:** A high-density operating manual for a complex Nx monorepo that defines architecture, behavioral principles, and environment requirements.

**Source credibility:** High; Supabase is an industry-standard developer tool with massive community trust and high maintenance.

**Recency:** Highly current, reflecting modern monorepo patterns (Nx) and recent repository activity.

**Source:** [supabase/supabase-js/.claude/CLAUDE.md](https://github.com/supabase/supabase-js/blob/a25062e9285fa8e3bd702c59ddda0d87ad1fcc27/.claude/CLAUDE.md) · 4475★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude AI Instructions for Supabase JS Libraries Monorepo

You are assisting with development in a unified Nx monorepo that consolidates all Supabase JavaScript SDKs, built with Nx for optimal developer experience and maintainability. This strategic migration from 6 separate repositories addresses critical maintenance overhead, dependency duplication, and release coordination challenges while maintaining **zero breaking changes** for consumers.

> **📚 Essential Documentation**: Always refer to these guides for detailed information:
>
> - **[CONTRIBUTING.md](../CONTRIBUTING.md)** - Development guidelines, commit format, PR process
> - **[TESTING.md](../docs/TESTING.md)** - Complete testing guide with Docker requirements
> - **[RELEASE.md](../docs/RELEASE.md)** - Release workflows and versioning strategy
> - **[MIGRATION.md](../docs/MIGRATION.md)** - Cross-cutting migration notes (one H2 per theme). Per-package migrations live at `packages/core/<package>/migrations/`.
> - **[SECURITY.md](../docs/SECURITY.md)** - Security policies and responsible disclosure

## Repository Architecture

### Monorepo Structure

```text
supabase-js/
├── packages/core/
│   ├── supabase-js/      # @supab
```

</details>
