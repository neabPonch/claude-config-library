---
name: dannote__figma-use
source: https://github.com/dannote/figma-use/blob/b6957832a5f2c4106e7796177879361a172205c2/SKILL.md
repo: dannote/figma-use
kind: skill
stars: 559
last_pushed: 2026-04-25T12:31:11Z
license: mit
score: 9
domains: [design-automation, web-frontend, cli-tools]
tags: [figma, ui-generation, jsx, automation]
curated: 2026-06-15
curated_by: config-scout
---

# dannote/figma-use — skill

**Why it's worth keeping:** The dual-mode (imperative/declarative) approach is highly efficient for LLMs; the detailed style shorthand mapping provides a clear, low-token way to describe complex layouts.

**Summary:** Enables an agent to control Figma via a CLI using both imperative commands and declarative JSX. It allows for programmatic creation, styling, and exporting of design components.

**Source credibility:** High; significant star count and recent maintenance (2 months ago).

**Recency:** Very current; perfectly suited for modern agentic workflows requiring tool-use bridging.

**Source:** [dannote/figma-use/SKILL.md](https://github.com/dannote/figma-use/blob/b6957832a5f2c4106e7796177879361a172205c2/SKILL.md) · 559★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: figma-use
description: Control Figma via CLI — create shapes, frames, text, components, set styles, layout, variables, export images. Use when asked to create/modify Figma designs or automate design tasks.
---

# figma-use

CLI for Figma. Two modes: commands and JSX.

```bash
# Commands
figma-use create frame --width 400 --height 300 --fill "#FFF" --layout VERTICAL --gap 16
figma-use create icon mdi:home --size 32 --color "#3B82F6"
figma-use set fill 1:23 "$Colors/Primary"

# JSX (props directly on elements, NOT style={{}})
echo '<Frame p={24} bg="#3B82F6" rounded={12}>
  <Text size={18} color="#FFF">Hello</Text>
</Frame>' | figma-use render --stdin --x 100 --y 100
```

## Before You Start

```bash
figma-use status  # Check connection
```

If not connected — start Figma with remote debugging:

```bash
# macOS
open -a Figma --args --remote-debugging-port=9222

# Windows
"%LOCALAPPDATA%\Figma\Figma.exe" --remote-debugging-port=9222

# Linux
figma --remote-debugging-port=9222
```

> Figma 126+ blocks remote debugging. Run `figma-use patch` once to fix, then restart Figma. Click **Always Allow** on the keychain prompt. Re-run after Figma updates.
>
> **Can't patch?** Use `fig
```

</details>
