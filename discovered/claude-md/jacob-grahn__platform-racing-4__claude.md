---
name: jacob-grahn__platform-racing-4__claude
source: https://github.com/jacob-grahn/platform-racing-4/blob/46faca4917f719c5256d659d53b0a45fa5ddd007/client/CLAUDE.md
repo: jacob-grahn/platform-racing-4
kind: claude-md
stars: 28
last_pushed: 2025-12-08T22:31:02Z
license: gpl-3.0
score: 7
domains: [game-development, godot]
tags: [godot, mcp-integration, gdscript]
curated: 2026-06-16
curated_by: config-scout
---

# jacob-grahn/platform-racing-4 — claude-md

**Why it's worth keeping:** The instruction to use the godot-docs MCP server is an excellent pattern for ensuring tool-use accuracy in niche engines. It also provides a clear headless export command which is useful for automated workflows.

**Summary:** Provides specialized guidance for using Godot-specific MCP tools and essential build/export commands.

**Source credibility:** Low-star individual project; likely used for personal development.

**Recency:** Current; references modern MCP (Model Context Protocol) patterns relevant to today's Claude Code environment.

**Source:** [jacob-grahn/platform-racing-4/client/CLAUDE.md](https://github.com/jacob-grahn/platform-racing-4/blob/46faca4917f719c5256d659d53b0a45fa5ddd007/client/CLAUDE.md) · 28★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Godot Documentation
- Use the godot-docs MCP server tools to look up Godot classes, methods, properties, and signals before writing code
- When encountering unfamiliar Godot APIs, use godot_search or godot_get_class for accurate documentation
- Examples: godot_search for finding APIs, godot_get_class for detailed class info

## Build Commands
- Run the game: Open project.godot in Godot Engine and press F5
- Build for web: `godot --headless --verbose --export-release "Web" $PWD/build/web/index.html`
- Tests: Run test scenes directly in Godot (open *_test.tscn files and press F5)

## Code Style
- Indentation: Tabs (not spaces)
- Line length: <100 characters
- File/variable/function names: snake_case
- Class/Node names: PascalCase
- Constants/Enums: UPPER_CASE
- Types: Use static typing for clarity: `var health: int = 0`
- Node references: Always use explicit typing: `@onready var label: Label = $Label`
- Signals: Connect using signal keyword and callable syntax
- Organization: Group code by type (constants, variables, functions)
- Functions: One blank line between f
```

</details>
