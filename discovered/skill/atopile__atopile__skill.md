---
name: atopile__atopile__skill
source: https://github.com/atopile/atopile/blob/619eda7f777558a3e500dbad9cc2941712881495/.claude/skills/frontend/SKILL.md
repo: atopile/atopile
kind: skill
stars: 3402
last_pushed: 2026-06-13T02:58:22Z
license: mit
score: 9
domains: [web-frontend, extension-development, fullstack-architecture]
tags: [react, vite, typescript, vscode-extension]
curated: 2026-06-15
curated_by: config-scout
---

# atopile/atopile — skill

**Why it's worth keeping:** It provides explicit 'Change Paths' for different modification types and enforces a strict schema-first contract workflow between backend and frontend.

**Summary:** Defines frontend development standards, architectural boundaries, and deployment workflows for the atopile extension ecosystem.

**Source credibility:** Highly credible; part of a popular (3400+ stars) and actively maintained hardware design tool repo.

**Recency:** Extremely current, utilizing modern tooling like Bun, Vite, and Pydantic.

**Source:** [atopile/atopile/.claude/skills/frontend/SKILL.md](https://github.com/atopile/atopile/blob/619eda7f777558a3e500dbad9cc2941712881495/.claude/skills/frontend/SKILL.md) · 3402★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: frontend
description: "Frontend standards for atopile extension webviews: architecture, contracts, design system, and testing workflow."
---

# Frontend Skill

Use this skill when building or modifying frontend features in atopile.
Default target is extension webviews (`ui-server` + `vscode-atopile`).

## Quick Start

Dependency install:

```bash
cd src/ui-server
bun install
```

Frontend-only loop (no backend integration):

```bash
cd src/ui-server
bun run dev
bun run test
bun run build
```

Webview integration loop (backend + Vite):

```bash
cd src/ui-server
./dev.sh
```

Extension package/install loop:

```bash
ato dev compile && ato dev install cursor
# or
ato dev compile && ato dev install vscode
```

Command reference:

- `bun install`: install/sync JS dependencies.
- `bun run dev`: start local Vite dev server (frontend-only iteration).
- `bun run test`: run local Vitest suite once.
- `bun run build`: run local `tsc && vite build`.
- `./dev.sh`: run backend + Vite for integration testing in browser.
- `ato dev compile`: build extension artifacts (default target `all`).
- `ato dev install cursor|vscode`: install latest built extension `.vsix`.
- `ato dev ui`: open a
```

</details>
