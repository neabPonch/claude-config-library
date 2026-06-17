---
name: netlify__cli
source: https://github.com/netlify/cli/blob/30ba6a1ed65af3045a1565cc3b87b27747b65e9e/CLAUDE.md
repo: netlify/cli
kind: claude-md
stars: 1888
last_pushed: 2026-06-15T09:39:01Z
license: mit
score: 9
domains: [cli-tools, backend-infrastructure]
tags: [architecture-patterns, command-guide, dev-workflows]
curated: 2026-06-15
curated_by: config-scout
---

# netlify/cli — claude-md

**Why it's worth keeping:** It maps out specific design patterns (Registry/BaseCommand) and implementation details like environment variable precedence, which are vital for AI reasoning in complex systems.

**Summary:** Provides highly detailed command variations for testing and development alongside an exhaustive architectural breakdown of the system.

**Source credibility:** Netlify is a top-tier industry player with significant community adoption and active maintenance.

**Recency:** Very current, utilizing modern tools like Vitest and Node 20.x.

**Source:** [netlify/cli/CLAUDE.md](https://github.com/netlify/cli/blob/30ba6a1ed65af3045a1565cc3b87b27747b65e9e/CLAUDE.md) · 1888★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Build and Development
- `npm run build` - Compiles TypeScript using `tsc --project tsconfig.build.json`
- `npm run dev` - Runs TypeScript compiler in watch mode
- `npm run clean` - Removes the `dist/` directory

### Testing
- `npm test` - Runs the full test suite (unit, integration, and e2e tests)
- `npm run test:unit` - Runs unit tests only with `vitest run tests/unit/`
- `npm run test:integration` - Runs integration tests with `vitest run --retry=3 tests/integration/`
- `npm run test:e2e` - Runs end-to-end tests with `vitest run --config vitest.e2e.config.ts`
- **Single test file**: `npm exec vitest -- run tests/unit/lib/account.test.ts`
- **Single test by name**: `npm exec vitest -- run tests/unit/lib/account.test.ts -t 'test name'`
- **Debug tests**: `DEBUG_TESTS=true npm exec vitest -- run [test-file] -t 'test name'`
- `npm run test:init` - Sets up test dependencies for various fixtures (Hugo, Next.js, monorepo)

### Code Quality
- `npm run lint` - Runs ESLint with cache
- `npm run lint:fix` - Runs ESLint and automatically fixes issu
```

</details>
