---
name: flowglad__flowglad__claude
source: https://github.com/flowglad/flowglad/blob/aad66f18960bab4ca5f9f261ce26cd50b023283f/platform/flowglad-next/claude.md
repo: flowglad/flowglad
kind: claude-md
stars: 1716
last_pushed: 2026-05-17T18:12:00Z
license: other
score: 9
domains: [backend-api, devops, testing]
tags: [bun, drizzle, guardrails, safety-checks, test-automation]
curated: 2026-06-15
curated_by: config-scout
---

# flowglad/flowglad — claude-md

**Why it's worth keeping:** Uses 'NEVER' constraints for high-risk actions and includes the `CLAUDECODE=1` optimization tip to reduce token noise/cost. It also clearly categorizes test isolation levels which prevents agent confusion during debugging.

**Summary:** Provides highly specific guardrails for database migrations and environment safety to prevent agent-led data destruction.

**Source credibility:** High; 1700+ stars, active maintenance within the last month, and a specialized toolset.

**Recency:** Current; includes specific optimizations for Claude Code environments.

**Source:** [flowglad/flowglad/platform/flowglad-next/claude.md](https://github.com/flowglad/flowglad/blob/aad66f18960bab4ca5f9f261ce26cd50b023283f/platform/flowglad-next/claude.md) · 1716★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Package Manager
**IMPORTANT**: This project uses `bun` as its package manager. ALWAYS use `bun` for all package management operations. Never use `npm` or `yarn`.

Examples:
- Install dependencies: `bun run install-packages` (N.B. - this project is in a monorepo but installs its own packages, hence the custom install script)
- Add a package: `bun add <package-name>`
- Build: `bun run build`
- Lint and typecheck: `bun run check`

## Environment Configuration (NODE_ENV)

This project uses a NODE_ENV-based environment system that automatically selects the correct `.env` file:

| NODE_ENV | Env File | Use Case |
|----------|----------|----------|
| `development` | `.env.development` | Local dev with Vercel credentials (DEFAULT) |
| `test` | `.env.test` | Running tests against local test database |
| `production` | `.env.production` | Production builds/deploys |

**Key behaviors:**
- **Development is the default** - When NODE_ENV is unset, it defaults to `development`
- **Test scripts auto-detect** - Scripts starting with "test" automatically use `.env.test`
- **Database safety check** - A preload script blocks execution if DATABASE_URL points to a non-local database (prevents acciden
```

</details>
