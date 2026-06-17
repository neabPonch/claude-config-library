---
name: nrwl__nx__skill
source: https://github.com/nrwl/nx/blob/958e60a8a85e6f4706a92c740d2b6ee18af6c734/.claude/skills/dist-build-migration/SKILL.md
repo: nrwl/nx
kind: skill
stars: 28918
last_pushed: 2026-06-14T17:18:48Z
license: mit
score: 9
domains: [cli-tools, devops, typescript]
tags: [migration, refactoring, monorepos, nx]
curated: 2026-06-15
curated_by: config-scout
---

# nrwl/nx — skill

**Why it's worth keeping:** Uses a critical 'Preflight' step to validate dependency graphs and provides high-precision 'Before/After' code templates for complex configuration changes.

**Summary:** A sophisticated migration skill that automates refactoring package structures to support local dist builds and modern ESM resolution.

**Source credibility:** Extremely high; derived from the official Nx (nrwl) repository, a industry standard for monorepo management.

**Recency:** 

**Source:** [nrwl/nx/.claude/skills/dist-build-migration/SKILL.md](https://github.com/nrwl/nx/blob/958e60a8a85e6f4706a92c740d2b6ee18af6c734/.claude/skills/dist-build-migration/SKILL.md) · 28918★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: dist-build-migration
description: Migrate an Nx package to build to a local dist/ directory with nodenext module resolution, exports map, and @nx/nx-source condition.
allowed-tools: Bash, Read, Glob, Grep, Agent, Edit, Write
---

# Migrate Package to Local Dist Build

You are migrating an Nx monorepo package from building to `../../dist/packages/<name>` to building locally to `packages/<name>/dist/`. This matches the pattern already used by `nx` and `devkit`.

## Argument

The user provides a package name (e.g., `js`, `webpack`, `angular`). The package lives at `packages/<name>/`.

## Steps

### 0. Preflight: check `workspace:*` deps for unmigrated packages

Read `packages/<name>/package.json` and list every `workspace:*` dep (in `dependencies`, `devDependencies`, `peerDependencies`).

For each such dep, look at the target package's `project.json`. If it does **not** override `release.version.manifestRootsToUpdate` to `["packages/{projectName}"]`, that target package is still on the old layout. You **must** migrate those packages too (apply this skill to each), in the same PR.

**Why:** With `preserveLocalDependencyProtocols: true` (the new pattern), `nx release version`
```

</details>
