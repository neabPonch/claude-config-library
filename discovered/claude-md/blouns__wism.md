---
name: blouns__wism
source: https://github.com/blouns/wism/blob/2332f73716b7f78785bb65550cd77b4f930fdc1a/CLAUDE.md
repo: blouns/wism
kind: claude-md
stars: 3
last_pushed: 2026-06-14T23:58:33Z
license: other
score: 7
domains: [game-dev, unity, csharp, architecture]
tags: [bootstrap, architectural-rules, structure]
curated: 2026-06-15
curated_by: config-scout
---

# blouns/wism — claude-md

**Why it's worth keeping:** Uses a 'Core Rule' to prevent architectural drift and includes actionable agent instructions like checking git status before editing.

**Summary:** Provides architectural orientation by separating deterministic logic from Unity presentation and establishes specific agent behavior rules.

**Source credibility:** Low star count (3), but active maintenance indicates it is a live, functional project structure.

**Recency:** Current; incorporates modern agentic workflows like skill usage and Git-based state inspection.

**Source:** [blouns/wism/CLAUDE.md](https://github.com/blouns/wism/blob/2332f73716b7f78785bb65550cd77b4f930fdc1a/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# WISM Claude Bootstrap

Use this file when Claude opens the public WISM repo.

## Orientation

WISM is a public C# and Unity strategy-game workspace. The design goal is to keep rules and deterministic game logic in `WismClient`, while Unity projects provide views, input, editor tooling, and human-facing workflows.

## Repo Layout

```text
wism/
├── WismClient/      # Core game engine, commands, AI, tests, shared contracts
├── WismUnity/       # Primary Unity game front end
├── WismCompanion/   # Unity companion shell
└── Prototype/       # Legacy prototypes; avoid extending
```

## Agent Bootstrap

- Codex should use the user-level `wism-workspace` skill when available.
- Claude should read the nearest `CLAUDE.md` in the active solution folder.
- All agents should inspect `git status --short --branch` before editing.

## Public Boundary

Do not add local paths, credentials, internal automation details, or non-public planning language to this public repo.

## Core Rule

Prefer WismClient for rules and deterministic state changes. Prefer Unity projects for presentation, editor tooling, input, and visual inspection.
```

</details>
