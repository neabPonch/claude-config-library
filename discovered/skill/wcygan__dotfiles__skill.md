---
name: wcygan__dotfiles__skill
source: https://github.com/wcygan/dotfiles/blob/af4ba505a1bd9e95506301f05c8a7bb2c337f049/config/codex/skills/deno-docs/SKILL.md
repo: wcygan/dotfiles
kind: skill
stars: 191
last_pushed: 2026-06-06T10:37:14Z
license: unknown
score: 8
domains: [cli-tools, runtime, web-development]
tags: [deno, documentation-routing, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# wcygan/dotfiles — skill

**Why it's worth keeping:** The 'Navigation Heuristics' section is an excellent way to guide agent reasoning, while the 'Quality Rules' enforce security-conscious patterns like avoiding broad permissions (-A).

**Summary:** Provides a highly structured workflow for navigating Deno documentation and applying runtime-specific best practices. It maps technical keywords to specific documentation categories to streamline agent research.

**Source credibility:** High; comes from a well-maintained and starred dotfiles repository.

**Recency:** Current; includes modern Deno standards such as JSR, npm specifiers, and deno.json configuration.

**Source:** [wcygan/dotfiles/config/codex/skills/deno-docs/SKILL.md](https://github.com/wcygan/dotfiles/blob/af4ba505a1bd9e95506301f05c8a7bb2c337f049/config/codex/skills/deno-docs/SKILL.md) · 191★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: deno-docs
description: Use when working with Deno runtime documentation, Deno CLI commands, deno.json/package.json configuration, TypeScript support, Node/npm compatibility, modules and imports, permissions, web development, testing, debugging, JSX, environment variables, or @std packages. Use official Deno docs as source of truth and load only the relevant reference file before giving precise guidance or changing Deno code.
---

# Deno Docs

Use this skill to route Deno runtime questions to the right official docs before giving implementation advice or editing code.

## Workflow

1. Identify the Deno topic in the user request, repo files, or command output.
2. Read `references/doc-map.md` only when the right official page is not obvious.
3. Fetch the current official page from `https://docs.deno.com/...` before making precise claims about CLI flags, config fields, permissions, APIs, examples, or recommended patterns.
4. When editing a project, inspect local context before changing code: `deno.json`, `deno.jsonc`, `package.json`, import specifiers, lockfiles, tasks, and the installed `deno --version` when available.
5. Verify with the narrowest meaningful Deno command fir
```

</details>
