---
name: elbwalker__walkerOS__skill
source: https://github.com/elbwalker/walkerOS/blob/3e1d7a71bba490b24b7f2183c33770f88be38418/skills/walkeros-understanding-development/SKILL.md
repo: elbwalker/walkerOS
kind: skill
stars: 339
last_pushed: 2026-06-11T09:34:41Z
license: mit
score: 9
domains: [monorepo, typescript, tooling]
tags: [onboarding, workflow, architecture-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# elbwalker/walkerOS — skill

**Why it's worth keeping:** It includes critical 'tribal knowledge' like the manual synchronization required between Zod schemas/TS interfaces and the specific error visibility contract for pipeline integrity.

**Summary:** Acts as a high-level project manual that defines strict development workflows, package hierarchies, and coding standards.

**Source credibility:** High; a well-structured, actively maintained open-source monorepo.

**Recency:** Current; utilizes modern patterns (Zod, TypeScript, Tsup) suitable for today's development environments.

**Source:** [elbwalker/walkerOS/skills/walkeros-understanding-development/SKILL.md](https://github.com/elbwalker/walkerOS/blob/3e1d7a71bba490b24b7f2183c33770f88be38418/skills/walkeros-understanding-development/SKILL.md) · 339★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: walkeros-understanding-development
description:
  Use when contributing to walkerOS, before writing code, or when unsure about
  project conventions. Covers build/test/lint workflow, XP principles, folder
  structure, and package usage.
---

# Understanding walkerOS Development

## Overview

walkerOS follows extreme programming principles with strict conventions. This
skill is your foundation before writing any code.

**Core principle:** DRY, KISS, YAGNI. Test first. Verify before claiming
complete.

## Commands

| Command                       | Purpose                                                  |
| ----------------------------- | -------------------------------------------------------- |
| `npm install`                 | Install all dependencies                                 |
| `npm run dev`                 | Watch mode for all packages                              |
| `npm run build`               | Build all packages                                       |
| `npm run verify:touched -- X` | L1: typecheck + lint + test for one package              |
| `npm run verify:affected`     | L2: same, only for packages affected since `origin/main` |
| `npm run test:smok
```

</details>
