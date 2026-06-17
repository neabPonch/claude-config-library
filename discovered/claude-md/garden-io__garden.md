---
name: garden-io__garden
source: https://github.com/garden-io/garden/blob/4e7128de8dfb5f38f76a5d005a65a78110be7553/CLAUDE.md
repo: garden-io/garden
kind: claude-md
stars: 3591
last_pushed: 2026-06-11T14:45:30Z
license: mpl-2.0
score: 7
domains: [cli-tools, devops]
tags: [typescript, mocha, kubernetes, npm]
curated: 2026-06-15
curated_by: config-scout
---

# garden-io/garden — claude-md

**Why it's worth keeping:** Includes specific command patterns for filtering tests with '-g' and a crucial manual fallback for running TypeScript type-checking if the binary is missing.

**Summary:** Provides essential operational commands for project structure, testing (unit/integration), and code quality enforcement.

**Source credibility:** Highly credible; 3.5k stars and active maintenance suggest professional-grade documentation standards.

**Recency:** Current and highly applicable to modern CLI development workflows.

**Source:** [garden-io/garden/CLAUDE.md](https://github.com/garden-io/garden/blob/4e7128de8dfb5f38f76a5d005a65a78110be7553/CLAUDE.md) · 3591★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Garden Development Guide

## Project Structure

- **core/** - Main Garden codebase (commands, config, graph, plugins, logger)
- **cli/** - CLI package that bundles core and plugins into the final executable
- **sdk/** - TypeScript plugin SDK for Garden plugin development
- **plugins/** - Bundled plugins (terraform, pulumi, jib, conftest, docker-compose)
- **docs/** - Documentation for docs.garden.io
- **scripts/** - Build, release, and dev automation scripts

## Development Workflow

Start watch-mode recompilation in the background (recommended):
```bash
npm run dev
```

Run Garden locally:
```bash
bin/garden
```

## Testing 

We use Mocha as our test framework.

Unit tests (from `core/` directory):
```bash
npm run test
npm run test -- -g "LoginCommand"  # filter by pattern
```

Integration tests (from `core/` directory):
```bash
npm run integ-local
npm run integ-local -- -g "pattern"  # filter by pattern
```

## Code Quality

Lint (errors only):
```bash
npm run lint -- --quiet
```

Type checking (from `core/` directory):
```bash
npm run check-types
```

If `npm run check-types` fails due to missing `tsc` binary, run directly:
```bash
node node_modules/typescript/lib/tsc.js -p co
```

</details>
