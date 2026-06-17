---
name: yorkie-team__yorkie-js-sdk
source: https://github.com/yorkie-team/yorkie-js-sdk/blob/ca6547e348fbb08ece90d8e48e1d41774f662c1c/CLAUDE.md
repo: yorkie-team/yorkie-js-sdk
kind: claude-md
stars: 158
last_pushed: 2026-06-13T16:07:40Z
license: apache-2.0
score: 9
domains: [web-frontend, typescript-monorepo, sdk]
tags: [monorepo, typescript, crdt, workflow]
curated: 2026-06-14
curated_by: config-scout
---

# yorkie-team/yorkie-js-sdk — claude-md

**Why it's worth keeping:** Includes an 'Always run before submitting' command string and explains core architectural patterns (CRDTs/JSON proxies) to ensure AI-generated code follows the design logic.

**Summary:** Provides a highly structured development workflow for a TypeScript monorepo including build requirements, package maps, and strict linting rules.

**Source credibility:** High; active repository with well-defined monorepo structure and clear documentation standards.

**Recency:** Current; mentions modern tooling like Vitest, pnpm, and MCP integration.

**Source:** [yorkie-team/yorkie-js-sdk/CLAUDE.md](https://github.com/yorkie-team/yorkie-js-sdk/blob/ca6547e348fbb08ece90d8e48e1d41774f662c1c/CLAUDE.md) · 158★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Yorkie JavaScript SDK

pnpm monorepo with multiple packages for building collaborative editing applications.

## Development Commands

```sh
pnpm i                       # Install (pnpm enforced)
pnpm sdk build               # Build core SDK
pnpm sdk build:proto         # Regenerate protobuf code (buf generate)
pnpm lint                    # ESLint with auto-fix (zero warnings enforced)

# Tests require a running Yorkie server:
docker compose -f docker/docker-compose.yml up --build -d
pnpm sdk test                # Run all SDK tests
pnpm sdk test test/integration/tree_test.ts  # Specific test file
```

Package filters: `pnpm sdk`, `pnpm react`, `pnpm schema`, `pnpm prosemirror`, `pnpm devtools`

## After Making Changes

Always run before submitting:
```sh
pnpm lint && pnpm sdk build && pnpm sdk test
```

## Project Docs

- **Design docs**: `docs/design/` for architectural context. New docs use [TEMPLATE.md](docs/design/TEMPLATE.md).
- **Task tracking**: `docs/tasks/active/` for in-progress, `docs/tasks/archive/` for completed. Use `YYYYMMDD-<slug>-{todo,lessons}.md` pairs.
- **Setup**: Husky manages git hooks. Run `pnpm install` to set up automatically.

## Packages

- **`sdk`**
```

</details>
