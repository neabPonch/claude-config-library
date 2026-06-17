---
name: crafter-station__elements
source: https://github.com/crafter-station/elements/blob/5ecc481d8187cbf47335d6aaadd86e948cd02a21/CLAUDE.md
repo: crafter-station/elements
kind: claude-md
stars: 504
last_pushed: 2026-05-17T00:16:54Z
license: mit
score: 9
domains: [web-frontend, ui-components]
tags: [architecture-first, nextjs, rule-driven]
curated: 2026-06-15
curated_by: config-scout
---

# crafter-station/elements — claude-md

**Why it's worth keeping:** The 'Intent Layer' pattern of reading localized documentation before modification is a highly effective technique for managing project-wide scale. It also utilizes specific negative constraints (e.g., 'never npm') to prevent toolchain drift.

**Summary:** Implements a hierarchical context strategy using local AGENTS.md files and enforces strict toolchain invariants.

**Source credibility:** Strong; 504 stars and recent maintenance indicate high-quality, professional code.

**Recency:** Very current, referencing Next.js 15 and modern OKLCH color systems.

**Source:** [crafter-station/elements/CLAUDE.md](https://github.com/crafter-station/elements/blob/5ecc481d8187cbf47335d6aaadd86e948cd02a21/CLAUDE.md) · 504★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Elements

Full-stack shadcn/ui components. Registry-based architecture for AI-native and developer tool components.

## Intent Layer

**Before modifying code in a subdirectory, read its AGENTS.md first** to understand local patterns and invariants.

| Area | Path | Tokens | Purpose |
|------|------|--------|---------|
| Registry | `registry/AGENTS.md` | ~282k | Component definitions, shadcn schema |
| Components | `src/components/AGENTS.md` | ~129k | UI primitives, site components |
| Content | `src/content/AGENTS.md` | ~48k | MDX docs, provider configs |

### Global Invariants

- All components follow shadcn/ui registry schema (`registry-item.json`)
- Use OKLCH color system for theming (not hex/hsl)
- Fumadocs with Vesper theme for documentation
- Bun for package management (never npm)
- Biome for linting/formatting (never ESLint/Prettier)

### Component Architecture

```
registry/default/blocks/{category}/{component-name}/
├── registry-item.json       # Schema, dependencies, metadata
└── components/elements/     # TSX implementation

src/components/ui/           # Base shadcn primitives
src/components/elements/     # Site-specific elements
src/content/components/      # MDX doc
```

</details>
