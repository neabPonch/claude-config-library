---
name: AeneasVerif__aeneas
source: https://github.com/AeneasVerif/aeneas/blob/bf13c42e7c34d07fc396baffad39c93023b12914/CLAUDE.md
repo: AeneasVerif/aeneas
kind: claude-md
stars: 809
last_pushed: 2026-06-15T05:52:10Z
license: apache-2.0
score: 9
domains: [agents-ai, compilers, formal-verification]
tags: [modular-instructions, skill-files, symlink-architecture]
curated: 2026-06-15
curated_by: config-scout
---

# AeneasVerif/aeneas — claude-md

**Why it's worth keeping:** Prevents context window bloat by segregating specialized expertise into discrete files; uses a single source of truth via symlinking for both humans and AI.

**Summary:** Implements a highly advanced modular 'Skill File' architecture where domain-specific instructions are maintained in documentation and symlinked to the agent's workspace.

**Source credibility:** High-quality, highly technical project with 809 stars and active maintenance.

**Recency:** Extremely current; explicitly mentions Claude Code and modern MCP tool integration.

**Source:** [AeneasVerif/aeneas/CLAUDE.md](https://github.com/AeneasVerif/aeneas/blob/bf13c42e7c34d07fc396baffad39c93023b12914/CLAUDE.md) · 809★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Aeneas — Lean Backend

Aeneas translates Rust programs to pure Lean code for formal verification.

## Skill Files

All detailed instructions for AI agents live in `documentation/skills/`. These are
the **source of truth** — they are symlinked to `.github/instructions/` (for GitHub
Copilot) and `.claude/skills/` (for Claude Code). **Always edit files in
`documentation/skills/`**; changes propagate automatically through the symlinks.

| Skill file | Covers |
|---|---|
| `aeneas-compiler-dev` | Dev workflow, formatting, tests, error macros, **skill file structure**, **build rules** |
| `aeneas-lean-core` | Translation model, spec patterns, tactic reference, pitfalls |
| `aeneas-tactics-quickref` | Tactic decision tree, banned tactics, combinations |
| `lean-lsp-mcp` | lean-lsp-mcp MCP tools for interactive proof development |
| `launching-proof-agents` | Multi-agent proof orchestration, review gates |
| `verification-campaigns` | Planning and executing large verification campaigns |
| `proof-patterns` | Worked proof examples (loops, dot products, comparisons) |
| `aeneas-crypto-verification` | Crypto-specific proof strategies (Montgomery, NTT, etc.) |

## Key Documentation

- `docum
```

</details>
