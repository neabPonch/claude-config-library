---
name: SAP__fundamental-ngx
source: https://github.com/SAP/fundamental-ngx/blob/ddc4254c63174d35fd3fef3b4c1504ab0b535da4/CLAUDE.md
repo: SAP/fundamental-ngx
kind: claude-md
stars: 292
last_pushed: 2026-06-15T15:28:52Z
license: apache-2.0
score: 9
domains: [web-frontend, angular]
tags: [anti-patterns, slash-commands, architectural-constraints]
curated: 2026-06-15
curated_by: config-scout
---

# SAP/fundamental-ngx — claude-md

**Why it's worth keeping:** The 'Landmines' section provides precise negative constraints to prevent common errors in modern Angular (signals vs legacy), and the 'Skills' table demonstrates how to define high-level automation via slash commands.

**Summary:** A highly structured guide for a modern Angular monorepo that defines architectural boundaries and strict technical constraints.

**Source credibility:** High; maintained by SAP with recent activity and enterprise-grade structure.

**Recency:** Highly current, referencing Angular 19/21+ features like signals and linkedSignal.

**Source:** [SAP/fundamental-ngx/CLAUDE.md](https://github.com/SAP/fundamental-ngx/blob/ddc4254c63174d35fd3fef3b4c1504ab0b535da4/CLAUDE.md) · 292★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Fundamental NGX

Angular component library (Angular 21+, NX monorepo, Yarn 4).
All components standalone by default.

## Architecture

NX monorepo with publishable libraries:

| Library                   | Scope tag                | Prefix | Purpose                                                   |
| ------------------------- | ------------------------ | ------ | --------------------------------------------------------- |
| `libs/core`               | `scope:fd`               | `fd-`  | Base UI components (button, dialog, card, calendar, etc.) |
| `libs/platform`           | `scope:fdp`              | `fdp-` | Higher-level composites built on core                     |
| `libs/cdk`                | `scope:cdk`              | `fdk-` | Utilities, forms, data-source abstractions                |
| `libs/btp`                | `scope:fdb`              | `fdb-` | Business Technology Platform components                   |
| `libs/cx`                 | `scope:cx`               | `cx-`  | Customer Experience components                            |
| `libs/i18n`               | `scope:i18n`             | —      | Internationalization (signal-based)                       |
| `libs/dateti
```

</details>
