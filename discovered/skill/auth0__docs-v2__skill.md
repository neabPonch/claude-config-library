---
name: auth0__docs-v2__skill
source: https://github.com/auth0/docs-v2/blob/6ab643487df0d5e5d1ba75193d5001f95d88bfbe/main/skill.md
repo: auth0/docs-v2
kind: skill
stars: 20
last_pushed: 2026-06-13T00:04:56Z
license: mit
score: 8
domains: [security, authentication, full-stack, mobile]
tags: [manifest, router-pattern, modular, auth]
curated: 2026-06-14
curated_by: config-scout
---

# auth0/docs-v2 — skill

**Why it's worth keeping:** Demonstrates the 'Router Pattern': using a single entry-point skill to detect context (framework/platform) and route the agent to highly specific sub-skills, preventing token bloat.

**Summary:** A high-level dispatcher manifest that organizes a massive suite of specialized authentication skills into logical categories like frontend, backend, and mobile.

**Source credibility:** Highly credible; produced by the official Auth0 engineering team.

**Recency:** Very current, including support for modern frameworks like Nuxt 3/4 and Vite.

**Source:** [auth0/docs-v2/main/skill.md](https://github.com/auth0/docs-v2/blob/6ab643487df0d5e5d1ba75193d5001f95d88bfbe/main/skill.md) · 20★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: Auth0
description: Use when adding authentication to any application — detects your framework, sets up Auth0, and provides production-ready integration guides for 25 frameworks and platforms.
license: Apache-2.0
metadata:
  author: Auth0 <support@auth0.com>
  version: "1.1.0"
  repository: https://github.com/auth0/agent-skills
---

# Auth0 Agent Skills

Auth0 provides AI agent skills for implementing authentication across any framework. Each skill contains best practices, code patterns, and step-by-step guidance tested against the latest Auth0 SDKs.

## Getting Started

Start here — this skill detects your framework and routes to the correct integration guide:

- **auth0-quickstart** — Framework detection and Auth0 setup

## Frontend Frameworks

- **auth0-react** — React SPAs (Vite, CRA) with `@auth0/auth0-react`
- **auth0-vue** — Vue.js 3 applications with `@auth0/auth0-vue`
- **auth0-angular** — Angular 13+ with `@auth0/auth0-angular`
- **auth0-spa-js** — Vanilla JS, Svelte, SolidJS, or any SPA with `@auth0/auth0-spa-js`

## Full-Stack Frameworks

- **auth0-nextjs** — Next.js App Router and Pages Router with `@auth0/nextjs-auth0`
- **auth0-nuxt** — Nuxt 3/4 applications
```

</details>
