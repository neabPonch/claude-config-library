---
name: Metaculus__metaculus
source: https://github.com/Metaculus/metaculus/blob/41be3899c234c2953b235a6c772c3dd586bef5c8/Claude.md
repo: Metaculus/metaculus
kind: claude-md
stars: 108
last_pushed: 2026-06-14T05:15:54Z
license: bsd-2-clause
score: 8
domains: [web-development, fullstack, django, nextjs]
tags: [monorepo, python, typescript, toolchain]
curated: 2026-06-14
curated_by: config-scout
---

# Metaculus/metaculus — claude-md

**Why it's worth keeping:** It provides high-value toolchain warnings (e.g., 'lint' includes type checking) and specific instructions for handling internationalization to prevent hardcoded strings.

**Summary:** A specialized configuration for a Django and Next.js monorepo that covers project structure, specific linting nuances, and translation workflows.

**Source credibility:** Metaculus is a highly reputable forecasting organization with an actively maintained codebase.

**Recency:** Very current; it utilizes modern-standard tools like `uv` and `bun`.

**Source:** [Metaculus/metaculus/Claude.md](https://github.com/Metaculus/metaculus/blob/41be3899c234c2953b235a6c772c3dd586bef5c8/Claude.md) · 108★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project structure
This is a Django + Next.js monorepo. Python/Django backend lives in the root directory, Next.js frontend lives in `front_end/`.

# Bash commands
- `cd ./front_end && bun run build`: Build the project
- `cd ./front_end && bun run format`: Format the frontend code
- `cd ./front_end && bun run lint`: Run linter AND type checker in parallel (includes both `lint:js` and `lint:types`). Do NOT run `lint` and `lint:types` separately — `lint` already includes type checking.
- `uv run ruff format .`: Format Python code
- `uv run ruff check .`: Lint Python code

# Code style
- Check the existing code style and follow it
- Destructure imports when possible (eg. import { foo } from 'bar')
- Do not use inline imports where possible. Prefer top-level imports.
- Do not add excessive comments. Add comments only to document what would be surprising to a senior engineer.
- For any frontend content visible to the user, use the translation mechanism used across the whole frontend. `const t = useTranslations()` and then `t("stringKey")` while adding the "stringKey" to all the corresponding language files in `front_end/messages/`: `en.json`, `es.json`, `cs.json`, `pt.json`, `zh.json`,
```

</details>
