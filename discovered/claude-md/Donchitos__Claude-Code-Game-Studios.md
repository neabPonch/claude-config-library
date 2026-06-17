---
name: Donchitos__Claude-Code-Game-Studios
source: https://github.com/Donchitos/Claude-Code-Game-Studios/blob/984023ddac0d5e27624f2baacde6105e45de375f/CLAUDE.md
repo: Donchitos/Claude-Code-Game-Studios
kind: claude-md
stars: 21681
last_pushed: 2026-05-21T23:33:07Z
license: mit
score: 9
domains: [game-dev, ai-agents, workflow-orchestration]
tags: [orchestration, protocol, multi-agent]
curated: 2026-06-15
curated_by: config-scout
---

# Donchitos/Claude-Code-Game-Studios — claude-md

**Why it's worth keeping:** The 'Question -> Options -> Decision -> Draft -> Approval' protocol is a gold-standard pattern for human-in-the-loop control. The use of structured documentation pointers provides a scalable way to manage large project contexts without bloating the main file.

**Summary:** An orchestration hub that manages complex game development through specialized sub-agents and modular documentation hierarchy.

**Source credibility:** High; highly starred repository indicating significant community validation and specialized utility.

**Recency:** Highly current; updated within the last month for modern Claude Code workflows.

**Source:** [Donchitos/Claude-Code-Game-Studios/CLAUDE.md](https://github.com/Donchitos/Claude-Code-Game-Studios/blob/984023ddac0d5e27624f2baacde6105e45de375f/CLAUDE.md) · 21681★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Game Studios -- Game Studio Agent Architecture

Indie game development managed through 49 coordinated Claude Code subagents.
Each agent owns a specific domain, enforcing separation of concerns and quality.

## Technology Stack

- **Engine**: [CHOOSE: Godot 4 / Unity / Unreal Engine 5]
- **Language**: [CHOOSE: GDScript / C# / C++ / Blueprint]
- **Version Control**: Git with trunk-based development
- **Build System**: [SPECIFY after choosing engine]
- **Asset Pipeline**: [SPECIFY after choosing engine]

> **Note**: Engine-specialist agents exist for Godot, Unity, and Unreal with
> dedicated sub-specialists. Use the set matching your engine.

## Project Structure

@.claude/docs/directory-structure.md

## Engine Version Reference

@docs/engine-reference/godot/VERSION.md

## Technical Preferences

@.claude/docs/technical-preferences.md

## Coordination Rules

@.claude/docs/coordination-rules.md

## Collaboration Protocol

**User-driven collaboration, not autonomous execution.**
Every task follows: **Question -> Options -> Decision -> Draft -> Approval**

- Agents MUST ask "May I write this to [filepath]?" before using Write/Edit tools
- Agents MUST show drafts or summaries
```

</details>
