---
name: JuliusBrussee__caveman-code__claude
source: https://github.com/JuliusBrussee/caveman-code/blob/d9a441eccda34626b5e1ae8bb081015986fdf4b0/packages/CLAUDE.md
repo: JuliusBrussee/caveman-code
kind: claude-md
stars: 491
last_pushed: 2026-06-05T20:34:48Z
license: mit
score: 7
domains: [cli-tools, agents-ai, typescript-monorepo]
tags: [monorepo, documentation-pattern, architecture-ssot]
curated: 2026-06-15
curated_by: config-scout
---

# JuliusBrussee/caveman-code — claude-md

**Why it's worth keeping:** Uses an authoritative 'master plan' file as a single source of truth for architecture and employs structured tables to help the agent map directories to specific packages/tools.

**Summary:** Defines a complex TypeScript monorepo structure with clear package-to-binary mappings and development conventions.

**Source credibility:** The repo is active and shows highly organized, professional developer tooling.

**Recency:** Very current; uses modern tools like Biome and targets a 'v2' iteration.

**Source:** [JuliusBrussee/caveman-code/packages/CLAUDE.md](https://github.com/JuliusBrussee/caveman-code/blob/d9a441eccda34626b5e1ae8bb081015986fdf4b0/packages/CLAUDE.md) · 491★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Packages

TypeScript monorepo under the `@juliusbrussee/caveman-*` scope on npm.

## Package Map

**v2 core (load-bearing — see `context/plans/cave-v2-best-in-class.md`):**

| Dir | Package | Binary | Role |
|-----|---------|--------|------|
| `coding-agent/` | `@juliusbrussee/caveman-code` | `caveman` / `caveman-code` | Main coding agent CLI |
| `ai/` | `@juliusbrussee/caveman-ai` | `pi-ai` | Multi-provider LLM unified API |
| `agent/` | `@juliusbrussee/caveman-agent` | — | Agent runtime: tool calling, state |
| `tui/` | `@juliusbrussee/caveman-tui` | — | Terminal UI: differential rendering |

**Out of scope for v2 (separate product surfaces):**

| Dir | Package | Binary | Role |
|-----|---------|--------|------|
| `web-ui/` | `@juliusbrussee/caveman-web-ui` | — | Web components for AI chat |
| `mom/` | `@juliusbrussee/caveman-mom` | `mom` | Slack bot → coding agent delegate |
| `pods/` | `@juliusbrussee/caveman-pods` | `cave-pods` | vLLM deployment on GPU pods |

## Conventions

- Read package-level README.md before modifying.
- Shared TypeScript config: `../tsconfig.base.json`.
- Biome for lint/format (not ESLint/Prettier).
- The active master plan is `context/plans/cave-v2-be
```

</details>
