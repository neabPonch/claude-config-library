---
name: CraftOS-dev__CraftBot__skill
source: https://github.com/CraftOS-dev/CraftBot/blob/6c3fac8926a82c7e880f5b3f79a5baac36754cfc/skills/cli-anything/SKILL.md
repo: CraftOS-dev/CraftBot
kind: skill
stars: 355
last_pushed: 2026-06-15T08:09:20Z
license: mit
score: 9
domains: [cli-tools, automation, media-processing]
tags: [harness-pattern, cross-platform, resilient-agents]
curated: 2026-06-15
curated_by: config-scout
---

# CraftOS-dev/CraftBot — skill

**Why it's worth keeping:** The 'Forbidden' section prevents OS-specific path/execution errors, while the fallback logic ensures task completion by transitioning from specialized tools to Python libraries if the primary tool fails.

**Summary:** Provides a cross-platform tool harness that abstracts complex media and productivity applications into predictable, agent-friendly actions.

**Source credibility:** High; 355 stars and very recent maintenance.

**Recency:** Current; utilizes advanced agentic patterns like tool abstraction and resilient fallbacks.

**Source:** [CraftOS-dev/CraftBot/skills/cli-anything/SKILL.md](https://github.com/CraftOS-dev/CraftBot/blob/6c3fac8926a82c7e880f5b3f79a5baac36754cfc/skills/cli-anything/SKILL.md) · 355★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cli-anything
description: "Automatically handles image editing, document conversion, audio/video editing, 3D rendering, diagrams, AI image generation, and more — using GIMP, LibreOffice, Blender, Audacity, Inkscape, Krita, Kdenlive, Shotcut, OBS, Draw.io, Mermaid, Ollama, Stable Diffusion, ComfyUI, JupyterLab, FreeCAD, QGIS, Grafana, Gitea, GitLab, NextCloud, Jenkins, AdGuard Home, Zoom, Mubu. User does NOT need to mention CLI-Anything — agent auto-selects the right app for the task. Auto-installs if not present."
action-sets: ["shell", "file_operations"]
---

# CLI-Anything Skill

**Core rule: Do everything yourself. Never give the user a command to run. Never explain steps. Just execute the task and report the result.**

**Activation rule: The user does NOT need to say "CLI-Anything". If their task matches a supported app below, use it automatically — no prompting needed.**

---

## Task Routing — Auto-select the right app (check this before every task)

| If the user asks about... | Use this app | Command prefix |
|---|---|---|
| Resize / crop / filter / edit an image | **GIMP** | `cli-anything-gimp` |
| Convert image format (JPG→PNG, PNG→WEBP, etc.) | **GIMP** | `cli-
```

</details>
