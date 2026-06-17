---
name: hoodoer__JS-Tap
source: https://github.com/hoodoer/JS-Tap/blob/05fb3e65b25b39ce128406e0bd117c197cde26d8/CLAUDE.md
repo: hoodoer/JS-Tap
kind: claude-md
stars: 455
last_pushed: 2026-06-11T16:23:53Z
license: unlicense
score: 8
domains: [web-frontend, security]
tags: [ui-consistency, css-constraints, build-instructions]
curated: 2026-06-15
curated_by: config-scout
---

# hoodoer/JS-Tap — claude-md

**Why it's worth keeping:** The use of 'NEVER' rules for colors is a top-tier technique to stop the AI from defaulting to generic or incorrect palettes. Mapping semantic classes to exact hex values ensures UI integrity across different components.

**Summary:** This file enforces strict visual consistency using specific hex codes and 'negative constraints' to prevent style drift. It also provides concrete, path-specific build instructions.

**Source credibility:** High; 455 stars and recent activity indicate a widely used, real-world security tool.

**Recency:** Current; includes modern development workflows like WXT and specific Python environment management.

**Source:** [hoodoer/JS-Tap/CLAUDE.md](https://github.com/hoodoer/JS-Tap/blob/05fb3e65b25b39ce128406e0bd117c197cde26d8/CLAUDE.md) · 455★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# JS-Tap Project Instructions

## UI Style Rules (MANDATORY)

Before creating or modifying ANY UI elements, read @STYLE_GUIDE.md.

This project uses Bootswatch **Slate** theme on Bootstrap 5.3. The palette is gray-toned, NOT blue-toned. Key rules:

- **Backgrounds**: `#272b30` (page), `#3a3f44` (cards/inputs). NEVER use blue-tinted darks like `#1a1a2e`, `#16213e`, `#0f3460`.
- **Text**: `#aaa` (body), `#fff` (emphasis/headings), `#7a8288` (muted/labels). NEVER use `#e0e0e0`.
- **Borders**: `#52565a` or `#6c757d`. NEVER use `#333`.
- **Buttons**: Use Bootstrap Slate semantic classes (`btn-primary`, `btn-outline-success`, `btn-outline-danger`, etc.). NEVER invent custom solid-fill button colors.
- **Badges**: Use `bg-success`, `bg-warning`, `bg-danger`, `bg-info`, `bg-secondary`, `bg-dark` on a `#272b30` background. NEVER use custom badge background colors.
- **Headings**: Always `#fff`. NEVER color headings cyan, blue, or any accent color.
- **Active indicators**: 3px left border using Slate semantic colors (`#62c462` success, `#f89406` warning). NEVER use full colored borders or custom highlight fills.
- **Status toast colors**: Match `showToast()` — `bg-success` (green), `bg-dange
```

</details>
