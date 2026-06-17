---
name: devlint__GitWand
source: https://github.com/devlint/GitWand/blob/1f583529bf20a6b0ae99b089dfac1b1b933253de/CLAUDE.md
repo: devlint/GitWand
kind: claude-md
stars: 100
last_pushed: 2026-06-11T22:35:51Z
license: mit
score: 9
domains: [monorepo-management, architectural-governance, fullstack]
tags: [monorepo, hierarchical-context, rule-delegation]
curated: 2026-06-15
curated_by: config-scout
---

# devlint/GitWand — claude-md

**Why it's worth keeping:** Demonstrates a sophisticated hierarchical documentation pattern where the root file delegates specific context to sub-directory CLAUDE.md files. It enforces strict dependency rules (e.g., prohibiting Node.js in core) to prevent architectural erosion during AI-driven development.

**Summary:** A high-level orchestration file that establishes architectural governance and technical constraints for a complex multi-package monorepo.

**Source credibility:** High; active repository with recent maintenance and a clearly defined professional tech stack.

**Recency:** Very current, utilizing modern standards like Tauri 2.

**Source:** [devlint/GitWand/CLAUDE.md](https://github.com/devlint/GitWand/blob/1f583529bf20a6b0ae99b089dfac1b1b933253de/CLAUDE.md) · 100★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
@AGENTS.md

## GitWand — Vue d'ensemble

GitWand est un client Git desktop natif avec un moteur de résolution automatique de conflits Git et des features AI intégrées.

**Stack technique :** Tauri 2, Vue 3, Rust, TypeScript, pnpm monorepo

**Versions actuelles :**

| Package | Nom npm | Version |
|---|---|---|
| `apps/desktop` | `@gitwand/desktop` | 2.9.0 |
| `packages/core` | `@gitwand/core` | 2.9.0 |
| `packages/cli` | `@gitwand/cli` | 2.9.0 |
| `packages/mcp` | `@gitwand/mcp` | 2.9.0 |
| `packages/vscode` | `gitwand-vscode` | 1.2.0 |

## Architecture monorepo

```
GitWand/
├── apps/
│   └── desktop/          # App Tauri 2 + Vue 3
├── packages/
│   ├── core/             # Moteur TS résolution conflits
│   ├── cli/              # CLI Node.js @gitwand/cli
│   ├── mcp/              # Serveur MCP @gitwand/mcp
│   └── vscode/           # Extension VS Code
├── website/              # Docs VitePress
├── scripts/
│   └── bump-version.sh   # Script de versioning
├── .github/workflows/    # CI/CD
└── AGENTS.md             # Règles AI transverses
```

### Séparation des responsabilités

- **`packages/core`** — moteur portable (browser/Node/Tauri), logique de résolution PURE. Aucune dépendan
```

</details>
