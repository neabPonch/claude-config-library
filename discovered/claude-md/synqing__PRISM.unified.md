---
name: synqing__PRISM.unified
source: https://github.com/synqing/PRISM.unified/blob/acf194126737c1b310723b29ba3d18a30f4354fb/CLAUDE.md
repo: synqing/PRISM.unified
kind: claude-md
stars: 0
last_pushed: 2025-10-23T13:50:11Z
license: unknown
score: 8
domains: [monorepo, architecture]
tags: [decision-making-framework, multi-project]
curated: 2026-06-16
curated_by: config-scout
---

# synqing/PRISM.unified — claude-md

**Why it's worth keeping:** The three-tier 'Authority' system prevents instruction conflicts across diverse sub-projects, while persona-based agent definitions provide clear operational boundaries for specific tasks.

**Summary:** Orchestrates a complex multi-project monorepo using a hierarchical decision-making framework (ADR) and strict documentation protocols.

**Source credibility:** Low social proof/stars, but demonstrates high-level architectural sophistication often found in mature engineering teams.

**Recency:** Highly relevant; utilizes persona-specific instructions optimized for current agentic AI workflows.

**Source:** [synqing/PRISM.unified/CLAUDE.md](https://github.com/synqing/PRISM.unified/blob/acf194126737c1b310723b29ba3d18a30f4354fb/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# PRISM.unified — Project Memory

Principles
- No restrictive CI or branch protections. If it builds locally, push it.
- Keep changes minimal and targeted to the request. No broad refactors unless asked.
- Avoid submodules and heavy new tooling without clear value.
- Never edit secrets (e.g., .env). Prefer sample files and docs.

Structure
- apps/PRISM.node — Node service
- apps/K1.Landing-Page — Web app/site
- apps/M5Stack.tab5 — Tab5 apps/UI
- firmware/PRISM.k1 — ESP32S3 firmware (PlatformIO/CMake)
- tools/LC_SelfContained — Utilities, scripts, templates
- shared/ — Cross-project assets (design tokens, schemas, docs)

Decision-Making Framework

PRISM uses a 3-tier Architecture Decision Record (ADR) system:

**Tier 1: Cross-Project Decisions** (`.taskmaster-root/`)
- Decisions affecting multiple projects (firmware + web, firmware + M5Stack, etc.)
- Examples: API contracts, communication protocols, design tokens
- Process: `cd .taskmaster-root && ./scripts/create-cross-project-adr.sh`
- Authority: Cross-project CANON takes precedence over project-specific decisions
- See: `.taskmaster-root/README.md` for full details

**Tier 2: Firmware Full Fortress** (`firmware/PRISM.k1/.taskmast
```

</details>
