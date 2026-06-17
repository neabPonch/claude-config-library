---
name: firecow__gitlab-ci-local
source: https://github.com/firecow/gitlab-ci-local/blob/98c657300d6db8cc111c8b2039d0ed4f1ae082f7/CLAUDE.md
repo: firecow/gitlab-ci-local
kind: claude-md
stars: 3946
last_pushed: 2026-06-09T09:52:26Z
license: mit
score: 8
domains: [cli-tools, devops]
tags: [bun, typescript, testing-optimization, build-system]
curated: 2026-06-15
curated_by: config-scout
---

# firecow/gitlab-ci-local — claude-md

**Why it's worth keeping:** Uses negative constraints ('Never run the full test suite') to prevent time-wasting agent loops and clarifies non-obvious build-to-runtime mappings.

**Summary:** Provides critical runtime constraints for Bun and specific instructions to optimize test execution speed.

**Source credibility:** High; highly starred repository with very recent maintenance.

**Recency:** Very current, utilizing modern tools like Bun and Vitest.

**Source:** [firecow/gitlab-ci-local/CLAUDE.md](https://github.com/firecow/gitlab-ci-local/blob/98c657300d6db8cc111c8b2039d0ed4f1ae082f7/CLAUDE.md) · 3946★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project: gitlab-ci-local

CLI tool to run GitLab CI pipelines locally. Written in TypeScript, built with Bun.

## Build & Runtime

- **Runtime**: Bun (not Node.js). All scripts use `bun`/`bun run`. Tests use vitest.
- **npm publish**: Still uses `npm publish --provenance` because Bun doesn't support provenance.
- **`bin` field**: Points to `dist/index.js` (Node.js-compatible bundle built by `bun run build:node`), not `src/index.ts`. This keeps `npm install -g` working without Bun.
- **Standalone binaries**: Built with `bun build --compile` for linux-amd64, linux-arm64, macos-x64, macos-arm64, win.
- **Version**: Hardcoded as `0.0.0` in `package.json`. CI replaces it via `sed` before build/publish. At runtime, `src/index.ts` reads it from `package.json` import.

## Testing

- **Never run the full test suite** (`bun run test`), it takes too long. Always run targeted tests: `bunx vitest run tests/test-cases/<name>/`
- **Timeout**: Configured in `vitest.config.ts` (`testTimeout: 60_000`).
- **Docker tests**: Tests under `dind-*` require Docker and are slow.
- **depcheck ignores**: `depcheck,@types/bun,@types/bun-types,vitest,@vitest/coverage-v8`

## Schema

- `src/schema.json` is fet
```

</details>
