---
name: maybites__NodeOSC
source: https://github.com/maybites/NodeOSC/blob/e981fd150248b2337c1b3d8139fabeb18b7e3573/CLAUDE.md
repo: maybites/NodeOSC
kind: claude-md
stars: 154
last_pushed: 2026-06-05T08:32:03Z
license: gpl-3.0
score: 9
domains: [blender-addons, python, tooling]
tags: [architecture, threading-model, dev-workflow]
curated: 2026-06-15
curated_by: config-scout
---

# maybites/NodeOSC — claude-md

**Why it's worth keeping:** It includes critical 'negative constraints' regarding thread safety (never modify bpy.data in worker threads) and provides exact property names for expression evaluation.

**Summary:** Provides a comprehensive technical map of the addon's architecture, including specific data structures and network protocols.

**Source credibility:** The project is actively maintained with recent commits.

**Recency:** Very current; includes modern development workflows like VSCode extension integration.

**Source:** [maybites/NodeOSC/CLAUDE.md](https://github.com/maybites/NodeOSC/blob/e981fd150248b2337c1b3d8139fabeb18b7e3573/CLAUDE.md) · 154★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

NodeOSC is a Blender addon (v2.4.1) enabling real-time OSC (Open Sound Control) communication between Blender and external applications via UDP. It supports both receiving (mapping OSC messages to Blender properties) and sending (broadcasting Blender property values as OSC messages).

No build system, package manager, or test runner — this is a traditional Blender addon. Development cycle is: edit files → reload addon in Blender (Edit > Preferences > Addons, or use a script reloader).

All OSC library dependencies are **vendored** inside `server/oscpy/` and `server/pythonosc/`. No `pip install` required.

## Installation / Development Setup

1. Symlink or copy this folder into Blender's addons directory: `<blender>/scripts/addons/NodeOSC/`
2. Enable the addon in Blender: Edit > Preferences > Add-ons > search "NodeOSC"
3. Optional: Install [Animation Nodes](https://github.com/JacquesLucke/animation_nodes) or [Sorcar](https://github.com/aachman98/Sorcar) for node integration

To reload after code changes without restarting Blender, use the [Blender
```

</details>
