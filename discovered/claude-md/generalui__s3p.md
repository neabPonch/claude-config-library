---
name: generalui__s3p
source: https://github.com/generalui/s3p/blob/d8d6dcac7f9c8a68c50c196400e9007bfbfd42f0/CLAUDE.md
repo: generalui/s3p
kind: claude-md
stars: 320
last_pushed: 2026-04-17T14:00:26Z
license: isc
score: 9
domains: [cli-tools, backend]
tags: [caffeinescript, edge-cases, testing-workflow]
curated: 2026-06-14
curated_by: config-scout
---

# generalui/s3p — claude-md

**Why it's worth keeping:** The 'Gotchas' section is world-class, preempting specific language/parser pitfalls that frequently trip up LLMs; it also includes explicit warnings about existing bugs to prevent incorrect fixes.

**Summary:** Provides specialized technical guidance for a CaffeineScript project, covering build workflows, MinIO integration, and Jest testing strategies.

**Source credibility:** Solid open-source project with 320 stars and recent activity (2 months ago).

**Recency:** Highly relevant for modern Node.js environments and tool-assisted development.

**Source:** [generalui/s3p/CLAUDE.md](https://github.com/generalui/s3p/blob/d8d6dcac7f9c8a68c50c196400e9007bfbfd42f0/CLAUDE.md) · 320★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# s3p — notes for Claude

Source is CaffeineScript (`.caf`). Build compiles to `build/`. Tests run from `build/` via Jest.

## Workflow
- `npm run build` — compile `source/**.caf` → `build/**.js`. Errors from CaffeineScript are clear; read the caret location.
- `npm test` — Jest against `build/`. Needs `NODE_OPTIONS=--experimental-vm-modules` (wired in) for AWS SDK v3 dynamic imports.
- `npm run test:coverage` — same + coverage report.
- MinIO: `docker compose up -d`. Integration tests require env: `S3_ENDPOINT=http://localhost:9000 AWS_ACCESS_KEY_ID=testAccessKey AWS_SECRET_ACCESS_KEY=testSecretKey AWS_REGION=us-east-1`. Without `S3_ENDPOINT`, integration tests auto-skip.
- Test scenarios share `source/test/MinioTestHelper.caf` — use `setupTestScenario` which handles bucket cleanup in `afterAll`.

## CLI → API
Every CLI command has `--api-example` that prints the equivalent `require('s3p').xxx({...})` call. Use this to understand how to drive the API from tests.

## CaffeineScript gotchas (things I've hit)

**Skim this before writing `.caf` — the parser is strict about layout.**

### Chained method calls
- Multi-line: leading dot on each continuation line.
  ```
  foo
  .replace a
```

</details>
