---
name: lightdash__lightdash__skill
source: https://github.com/lightdash/lightdash/blob/7e84f03c5fba0d3456523c075cdf102e993c9d0d/.claude/skills/ld-permissions/SKILL.md
repo: lightdash/lightdash
kind: skill
stars: 5892
last_pushed: 2026-06-15T09:31:16Z
license: other
score: 9
domains: [security, backend-api, database]
tags: [authorization, casl, permissions, migrations]
curated: 2026-06-15
curated_by: config-scout
---

# lightdash/lightdash — skill

**Why it's worth keeping:** Includes an exceptional 'Migration Impact Table' that predicts how code changes (renaming/splitting scopes) affect the database, preventing silent permission loss.

**Summary:** Provides deep context for a complex CASL-based authorization system, covering scope definitions, code implementation patterns, and critical database migration requirements.

**Source credibility:** High; sourced from Lightdash, a highly starred and actively maintained open-source BI tool.

**Recency:** Current; uses modern TypeScript patterns and detailed migration strategies relevant to contemporary development.

**Source:** [lightdash/lightdash/.claude/skills/ld-permissions/SKILL.md](https://github.com/lightdash/lightdash/blob/7e84f03c5fba0d3456523c075cdf102e993c9d0d/.claude/skills/ld-permissions/SKILL.md) · 5892★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ld-permissions
description: Guide for Lightdash's CASL-based authorization system. Use when working with scopes, custom roles, abilities, permissions, ForbiddenError, authorization, or access control. Helps with adding new scopes, debugging permission issues, understanding the permission flow, and creating custom roles.
allowed-tools: Read, Grep, Glob, Task
---

# Permissions & Authorization Guide

This skill helps you work with Lightdash's CASL-based permissions system, including scopes, custom roles, and authorization enforcement.

## What do you need help with?

1. **Add a new scope/permission** - Step-by-step guide to add a new permission
2. **Debug a permission issue** - Troubleshoot why a user can't access something
3. **Understand the permission flow** - Learn how permissions work end-to-end
4. **Work with custom roles** - Create or modify custom roles with specific scopes

## Quick Reference

### Key Files

| Purpose | Location |
|---------|----------|
| Scope definitions | `packages/common/src/authorization/scopes.ts` |
| CASL types | `packages/common/src/authorization/types.ts` |
| Ability builder | `packages/common/src/authorization/index.ts` |
| System role ab
```

</details>
