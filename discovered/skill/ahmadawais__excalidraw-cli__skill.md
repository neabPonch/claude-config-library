---
name: ahmadawais__excalidraw-cli__skill
source: https://github.com/ahmadawais/excalidraw-cli/blob/d62ab7af3d7e7985724e80fa64a2253771a2513a/skills/skill.md
repo: ahmadawais/excalidraw-cli
kind: skill
stars: 76
last_pushed: 2026-02-11T18:45:41Z
license: unknown
score: 9
domains: [cli-tools, visual-generation, documentation]
tags: [excalidraw, diagramming, cli]
curated: 2026-06-16
curated_by: config-scout
---

# ahmadawais/excalidraw-cli — skill

**Why it's worth keeping:** Includes critical spatial and aesthetic heuristics like Z-order instructions, font size hierarchies, color palettes, and precise arrow-binding math.

**Summary:** A comprehensive technical specification for generating complex hand-drawn diagrams via the excalidraw-cli using JSON.

**Source credibility:** High; authored by a known developer for a specialized CLI utility.

**Recency:** Current; specifically optimized for high-fidelity 'diagrams-as-code' workflows used by modern agents.

**Source:** [ahmadawais/excalidraw-cli/skills/skill.md](https://github.com/ahmadawais/excalidraw-cli/blob/d62ab7af3d7e7985724e80fa64a2253771a2513a/skills/skill.md) · 76★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Excalidraw CLI — Agent Skill

Create hand-drawn diagrams from JSON using `excalidraw-cli`. Outputs `.excalidraw` files and shareable URLs.

## Quick Start

```bash
# Create diagram from inline JSON
excalidraw create --json '[...elements...]' -o diagram.excalidraw

# Export to shareable URL
excalidraw export diagram.excalidraw
# → https://excalidraw.com/#json=abc,key

# Create from file
excalidraw create elements.json -o diagram.excalidraw

# Pipe from stdin
echo '[...elements...]' | excalidraw create -o diagram.excalidraw
```

## Built-in Defaults (skip these in JSON)

The CLI auto-applies these so you write less JSON:

| Property | Default | Applies To |
|----------|---------|------------|
| `roughness` | `2` (sloppy/hand-drawn) | Shapes, arrows |
| `roundness` | `{ "type": 3 }` (rounded corners) | Shapes |
| `fontFamily` | `1` (Excalifont/Virgil handwritten) | Text |
| `strokeColor` | `"#1e1e1e"` | All |
| `backgroundColor` | `"transparent"` | All |
| `fillStyle` | `"solid"` | All |
| `strokeWidth` | `2` | All |
| `opacity` | `100` | All |

Override any default by setting it explicitly.

## Element Types

### Shapes (rectangle, ellipse, diamond)

Minimal — just type, id, positi
```

</details>
