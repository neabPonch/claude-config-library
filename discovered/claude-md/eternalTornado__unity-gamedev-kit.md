---
name: eternalTornado__unity-gamedev-kit
source: https://github.com/eternalTornado/unity-gamedev-kit/blob/c0513391aed54f5827d0bd641e526a8f9f3c1640/CLAUDE.md
repo: eternalTornado/unity-gamedev-kit
kind: claude-md
stars: 0
last_pushed: 2026-04-16T10:03:56Z
license: mit
score: 9
domains: [game-development, unity, csharp]
tags: [workflow-driven, path-scoped-rules, phase-gated, unity-6]
curated: 2026-06-16
curated_by: config-scout
---

# eternalTornado/unity-gamedev-kit — claude-md

**Why it's worth keeping:** Uses advanced patterns like path-scoped rule delegation (linking folders to specific `.md` rules) and incremental document construction to manage context limits. The phase-gate workflow is an excellent template for preventing AI drift in complex builds.

**Summary:** Establishes a highly structured, phase-gated development lifecycle specifically for Unity/C# projects. It integrates rigorous manual approval protocols and formal state management via 'gate checks' and session files.

**Source credibility:** The zero stars suggest a niche or new project, but the technical sophistication of the instructions indicates high-level expertise in Unity architecture.

**Recency:** Very current; references Unity 6 and modern C# constraints optimized for Claude Code's agentic capabilities.

**Source:** [eternalTornado/unity-gamedev-kit/CLAUDE.md](https://github.com/eternalTornado/unity-gamedev-kit/blob/c0513391aed54f5827d0bd641e526a8f9f3c1640/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Unity GameDev Kit

This project was bootstrapped with [`unity-gamedev-kit`](https://github.com/eternalTornado/unity-gamedev-kit).

## Role

You are Claude Code working inside a Unity game project. You follow a 5-phase workflow (Concept → Systems Design → Architecture → Implementation → Polish), with formal gates between phases. Phase 4 (Implementation) delegates to [speckit](https://github.com/github/spec-kit) for `/plan` → `/tasks` → `/implement`.

## Collaboration Protocol

**User-driven collaboration, not autonomous execution.**

Every task: **Question → Options → Decision → Draft → Approval**.

- Ask *"May I write this to `<filepath>`?"* before every `Write` or `Edit`.
- Show drafts or summaries before requesting approval.
- Multi-file changes require explicit approval for the full changeset.
- **No git commits without user instruction.**

## Priority Hierarchy (for every code review)

1. 🔴 **Code Quality** — nullable types ON, zero warnings, throw not log, `nameof`, `readonly`/`const`, no inline comments.
2. 🟡 **Modern C#** — LINQ over loops, expression bodies, pattern matching, `??`/`?.`/`??=`, records.
3. 🟢 **Unity Architecture** — VContainer DI, SignalBus even
```

</details>
