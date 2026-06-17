---
name: MarkJamesHoward__Visual-Git
source: https://github.com/MarkJamesHoward/Visual-Git/blob/4fd522746ff4919772ebc7b4bbed68cab336549b/claude.md
repo: MarkJamesHoward/Visual-Git
kind: claude-md
stars: 2
last_pushed: 2026-05-03T00:33:05Z
license: unknown
score: 7
domains: [cli-tools, web-development]
tags: [command-override, project-structure, tooling]
curated: 2026-06-15
curated_by: config-scout
---

# MarkJamesHoward/Visual-Git — claude-md

**Why it's worth keeping:** Demonstrates how to prevent model errors by explicitly overriding standard tools (git -> tgit) and shows how to cross-reference specialized sub-directory instructions.

**Summary:** Establishes a critical command-line tool override and defines multi-module project structure.

**Source credibility:** Low star count but the specific tooling requirement suggests a real, non-generic project context.

**Recency:** Highly current based on recent push history.

**Source:** [MarkJamesHoward/Visual-Git/claude.md](https://github.com/MarkJamesHoward/Visual-Git/blob/4fd522746ff4919772ebc7b4bbed68cab336549b/claude.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Visual Git Project - Development Notes

## Git Operations

**IMPORTANT**: Use `tgit` instead of `git` for all git operations in this repository.

```bash
# Use this:
tgit status
tgit add .
tgit commit -m "message"
tgit push

# Not this:
git status  # ❌
```

## Project Structure

- `/cli` - Command line application (C# .NET)
- `/web` - Website (Astro framework)
- `/api` - Backend API (C# .NET)

## Additional Documentation

- See [web/claude.md](web/claude.md) for website-specific development notes (mimic.css workflow, styling conventions)
```

</details>
