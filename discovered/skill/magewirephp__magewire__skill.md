---
name: magewirephp__magewire__skill
source: https://github.com/magewirephp/magewire/blob/a7e33a651a7c40925834759e5b13d3c8e2f4300d/.claude/skills/magewire-architecture/SKILL.md
repo: magewirephp/magewire
kind: skill
stars: 260
last_pushed: 2026-06-14T15:13:59Z
license: mit
score: 9
domains: [php, magento-2, framework-architecture]
tags: [architecture, lifecycle, debugging-guide]
curated: 2026-06-15
curated_by: config-scout
---

# magewirephp/magewire — skill

**Why it's worth keeping:** Provides highly specific 'Footgun' warnings that prevent common DI errors and clearly defines boundaries between generated and hand-written code.

**Summary:** Detailed technical blueprint covering the framework's dual-layer architecture, runtime state machine, and service boot lifecycle.

**Source credibility:** Authored by the lead developer of Magewire (Willem Poortman) and is actively maintained.

**Recency:** Current; reflects modern PHP framework patterns and complex dependency injection lifecycles.

**Source:** [magewirephp/magewire/.claude/skills/magewire-architecture/SKILL.md](https://github.com/magewirephp/magewire/blob/a7e33a651a7c40925834759e5b13d3c8e2f4300d/.claude/skills/magewire-architecture/SKILL.md) · 260★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: magewire-architecture
description: "Internals and extension guide for the Magewire framework: directory layout (src/lib/dist/portman), Mechanisms vs Features, area-scoped DI (frontend/adminhtml), snapshot/state flow, layout containers, JS extension points, and Facades. Use when extending Magewire, creating custom Features or Mechanisms, debugging the framework itself, or understanding how the codebase is structured."
license: MIT
metadata:
  author: Willem Poortman
---

# Magewire Architecture

Magewire's codebase is split into two layers: an upstream Livewire core (PHP, ported and maintained via Portman) and a Magento integration layer (controllers, blocks, DI, layout, templates). Understanding this split is essential for knowing where to add or change things.

---

## Repository Layout

```
vendor/magewirephp/magewire/
├── src/                        # Magento module structure (hand-written, must live here for Magento)
│   ├── Component.php           # Base component class (public API)
│   ├── MagewireServiceProvider.php
│   ├── Controller/             # Route controllers (magewire/update)
│   ├── Model/                  # Magento-specific models, view utils, fragment h
```

</details>
