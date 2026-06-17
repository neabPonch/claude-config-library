---
name: Artmann__Centaur
source: https://github.com/Artmann/Centaur/blob/b90fe2c3fbb714143674e9715305e0ce3520b352/CLAUDE.md
repo: Artmann/Centaur
kind: claude-md
stars: 1
last_pushed: 2026-05-26T08:15:04Z
license: mit
score: 8
domains: [.net, desktop-app, graphics-rendering]
tags: [architectural-patterns, error-handling-protocol, domain-logic]
curated: 2026-06-16
curated_by: config-scout
---

# Artmann/Centaur — claude-md

**Why it's worth keeping:** It explains specific technical 'gotchas' (like immediate-mode rendering) to prevent incorrect optimizations and enforces a strict error-handling workflow tied to UI notifications.

**Summary:** Provides deep architectural context for an Avalonia-based terminal, covering custom extension patterns and rendering constraints.

**Source credibility:** Low star count, but the high density of domain-specific technical logic indicates an experienced developer's hand.

**Recency:** Current; it serves as an excellent example of providing 'guardrails' for LLM-driven development.

**Source:** [Artmann/Centaur/CLAUDE.md](https://github.com/Artmann/Centaur/blob/b90fe2c3fbb714143674e9715305e0ce3520b352/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
- Don't use CONSTANT_CASE. Use camelCase or PascalCase for variables and functions.
- Don't include Claude in the commits

## Formatting and Linting

- **CSharpier** for formatting: `dotnet csharpier format .`
- **Roslyn Analyzers** for linting: runs automatically during `dotnet build`
- Run `dotnet csharpier check .` to verify formatting without writing changes
- CSharpier is a local dotnet tool — run `dotnet tool restore` after cloning

## Commit Messages

- Don't include Claude as the author in commit messages

## Avalonia Rendering

- Avalonia uses **immediate-mode rendering** - each frame receives a fresh canvas
- The canvas is NOT preserved between frames (starts cleared/transparent)
- Incremental/dirty-region rendering doesn't work with `ICustomDrawOperation.Render()` because unchanged areas won't be redrawn
- Always do full redraws in custom draw operations
- Timer-based update coalescing (batching multiple updates into one render) is still useful for reducing flicker from rapid PTY output

## Extension & Provider Pattern

The codebase uses an **ExtensionHost** (`Centaur.Core.Hosting`) to manage component lifecycle and extensibility.

### Extensions (activate/dispose)

- Im
```

</details>
