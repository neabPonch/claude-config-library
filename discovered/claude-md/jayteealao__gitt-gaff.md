---
name: jayteealao__gitt-gaff
source: https://github.com/jayteealao/gitt-gaff/blob/44bd313985b2e74dfe3b46fff32cb3f31dadd5fa/Claude.md
repo: jayteealao/gitt-gaff
kind: claude-md
stars: 0
last_pushed: 2026-01-09T13:48:51Z
license: unknown
score: 8
domains: [typescript, web-development]
tags: [strict-typing, technical-debt-prevention, engineering-standards]
curated: 2026-06-14
curated_by: config-scout
---

# jayteealao/gitt-gaff — claude-md

**Why it's worth keeping:** The 'No parallel implementations' rule prevents AI-generated bloat, while the 'Before you finish' checklist creates a strong ritual for cleaning up the workspace.

**Summary:** A strict engineering manifest for TypeScript projects that enforces architectural integrity and prevents technical debt. It emphasizes single sources of truth and the removal of legacy code during feature implementation.

**Source credibility:** Low based on repository metrics (0 stars), but the content demonstrates high engineering maturity.

**Recency:** Very current; aligns with modern TypeScript patterns and agentic workflow requirements.

**Source:** [jayteealao/gitt-gaff/Claude.md](https://github.com/jayteealao/gitt-gaff/blob/44bd313985b2e74dfe3b46fff32cb3f31dadd5fa/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — TypeScript repo (strict, clear, production)

Start: say hi. One motivating line. Then work.

## Owner / contact
- Owner: <FILL ME> (name, handle, email).

## Style goals (always)
- Simple, clear, readable. Production-grade.
- Prefer explicit code over clever tricks.
- Small functions, clear names, clear data flow.
- Keep types honest. Delete dead code. One source of truth.

## Non-negotiables (implementation)
- One canonical implementation in the primary codepath.
  - Remove legacy/shims/adapters in the same change.
  - No compatibility wrappers.
- Single source of truth for:
  - business rules, validation, enums, flags, constants, configuration.
- If frontend: UI thin view layer. Business rules live in domain/shared layer.
- Validate and sanitize all user-controlled input before OS/file/process/eval.
- Errors are explicit:
  - no silent catches.
  - user-visible error states where appropriate.
  - logs have context, no secrets.

## Workflow
- No git worktrees unless user asks.
  - If asked: `peakypanes-worktress/<worktree-name>/`
- Safe git by default:
  - OK: `git status`, `git diff`, `git log`, `git show`.
  - No destructive ops unless explicit.
  - No amend unless
```

</details>
