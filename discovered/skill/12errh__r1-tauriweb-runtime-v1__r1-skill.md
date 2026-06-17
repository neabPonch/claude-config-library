---
name: 12errh__r1-tauriweb-runtime-v1__r1-skill
source: https://github.com/12errh/r1-tauriweb-runtime-v1/blob/9309bc3627007f1b10afa41b4b25fbbccc8fbddf/PROMTS%20AND%20SKILL/R1_SKILL.md
repo: 12errh/r1-tauriweb-runtime-v1
kind: skill
stars: 8
last_pushed: 2026-05-03T15:12:59Z
license: agpl-3.0
score: 9
domains: [wasm, rust, web-runtime, cli-tools]
tags: [agent-instructions, architecture-guide, dependency-management]
curated: 2026-06-16
curated_by: config-scout
---

# 12errh/r1-tauriweb-runtime-v1 — skill

**Why it's worth keeping:** It uses a 'Critical rules' section to prevent architectural anti-patterns and a detailed version matrix to ensure the agent selects correct, compatible package versions.

**Summary:** A high-density AI knowledge base for the R1 Tauri runtime that provides strict architectural guardrails and precise dependency mapping.

**Source credibility:** Low star count (8) but demonstrates highly professional structural knowledge and specific technical detail.

**Recency:** Very current; includes compatibility for Vite 7 and modern toolchains.

**Source:** [12errh/r1-tauriweb-runtime-v1/PROMTS AND SKILL/R1_SKILL.md](https://github.com/12errh/r1-tauriweb-runtime-v1/blob/9309bc3627007f1b10afa41b4b25fbbccc8fbddf/PROMTS%20AND%20SKILL/R1_SKILL.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# R1 TauriWeb Runtime — AI Agent Skill (v0.3.7)

> This file is the complete knowledge base for any AI agent working with R1.
> Read this entire file before making any changes to the R1 project.
> Every decision you make must be consistent with the rules in this document.

---

## What R1 Is

R1 is a browser-native runtime for Tauri applications. It compiles a Tauri
app's Rust backend to WebAssembly and runs it entirely in the browser — no
server, no installer, no native binary. The end user visits a URL and the
full Tauri app works in their browser tab.

```
Developer's Tauri App (Rust + React/Svelte/Vue)
         ↓  npm run build  (with R1 Vite plugin)
         ↓
Static folder (HTML + JS + .wasm)
         ↓  deploy to Vercel / Netlify / GitHub Pages
         ↓
End user visits URL → full app runs in browser
```

---

## Current Status (v0.3.7 - April 2026)

✅ **PRODUCTION READY - ALL PACKAGES PUBLISHED**

- **npm packages:** `@r1-runtime/*` (7 packages)
- **crates.io:** `r1-macros` v0.3.0
- **Tests:** 105+ passing
- **SQLite:** Full support with OPFS persistence
- **CLI:** `npx @r1-runtime/cli sync` for automatic migration

### Package Versions
| Package | Version | Notes |
|---|-
```

</details>
