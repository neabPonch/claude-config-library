---
name: WayBetterDigital__dom-pl-marketplace-demo
source: https://github.com/WayBetterDigital/dom-pl-marketplace-demo/blob/ad9c2f177a2ce4c9485ef576bab2f8b3c25d5b26/CLAUDE.md
repo: WayBetterDigital/dom-pl-marketplace-demo
kind: claude-md
stars: 1
last_pushed: 2026-05-11T16:04:17Z
license: unknown
score: 8
domains: [web-frontend, backend-api, agents-ai]
tags: [skill-mapping, architectural-patterns, service-layer, nuxt-4, medusa-v2]
curated: 2026-06-15
curated_by: config-scout
---

# WayBetterDigital/dom-pl-marketplace-demo — claude-md

**Why it's worth keeping:** Uses a specialized 'Skill Mapping' table to manage context/tools and provides explicit code examples for enforcing service-layer boundaries.

**Summary:** A highly structured guide that uses tool-based 'skills' and strict architectural patterns to govern LLM behavior.

**Source credibility:** Low star count, but demonstrates high-level technical architecture typical of professional engineering.

**Recency:** Very current; uses latest versions of Nuxt (v4) and Medusa (v2).

**Source:** [WayBetterDigital/dom-pl-marketplace-demo/CLAUDE.md](https://github.com/WayBetterDigital/dom-pl-marketplace-demo/blob/ad9c2f177a2ce4c9485ef576bab2f8b3c25d5b26/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Agent Guide

## What this project is

A headless e-commerce store. The backend is **Medusa v2** (Node.js, TypeScript) running in Docker with PostgreSQL. The frontend is **Nuxt 4** with **@nuxt/ui v4** (Tailwind-based component library). They communicate via the Medusa JS SDK (`@nuxtjs/medusa`).

---

## Using LLM Skills

This project has skills that must be loaded before doing certain work. Always load the relevant skill before planning or writing code — skills contain architectural rules that override generic assumptions.

| Task | Skill to load |
|---|---|
| Medusa backend (modules, routes, workflows, data models) | `/medusa-dev:building-with-medusa` |
| Storefront API calls, SDK usage, data fetching | `/medusa-dev:building-storefronts` |
| Admin dashboard UI (widgets, custom pages) | `/medusa-dev:building-admin-dashboard-customizations` |
| Database migrations | `/medusa-dev:db-migrate` |
| Generate migration files | `/medusa-dev:db-generate` |
| Nuxt UI components, theming, layouts | `/nuxt-ui` |

Also use the **MedusaDocs MCP tool** (`mcp__plugin_medusa-dev_MedusaDocs__ask_medusa_question`) to look up Medusa-specific APIs, module patterns, and configuration options.

---

##
```

</details>
