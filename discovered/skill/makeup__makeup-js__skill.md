---
name: makeup__makeup-js__skill
source: https://github.com/makeup/makeup-js/blob/0e8afabe78dffae2f08ae9ef0c00e5190e2099d0/.claude/skills/release-module/skill.md
repo: makeup/makeup-js
kind: skill
stars: 47
last_pushed: 2026-06-12T20:10:45Z
license: mit
score: 9
domains: [cli-tools, devops, web-frontend]
tags: [lerna, monorepo, npm, release-automation]
curated: 2026-06-15
curated_by: config-scout
---

# makeup/makeup-js — skill

**Why it's worth keeping:** Demonstrates excellent 'human-in-the-loop' design by explicitly handing off interactive 2FA/OTP steps to the user; includes specific recovery instructions for common Lerna git errors.

**Summary:** Orchestrates a complex Lerna monorepo release workflow including verification, testing, and versioning.

**Source credibility:** Niche tool with active maintenance indicated by recent push dates.

**Recency:** Highly relevant; follows modern terminal-interactive agent patterns.

**Source:** [makeup/makeup-js/.claude/skills/release-module/skill.md](https://github.com/makeup/makeup-js/blob/0e8afabe78dffae2f08ae9ef0c00e5190e2099d0/.claude/skills/release-module/skill.md) · 47★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
description: Release changed packages with automatic Lerna detection and npm publish
args: [version-type] or [module-name] [version-type]
---

You are releasing packages in the makeup-js monorepo using Lerna's automatic change detection.

# Input

The user can provide:

**Automatic mode (recommended):**

- Just the version type: `patch` (default), `minor`, or `major`
- Lerna automatically detects all packages that have changed since the last release

**Targeted mode:**

- A specific module name (e.g., "makeup-listbox") AND version type
- Useful when you want to force-release a specific package even if Lerna doesn't detect changes

If no arguments are provided, defaults to `patch` for all changed packages.

# Process

## 1. Verify prerequisites

Before starting the release:

- Ensure all changes are committed (`git status` should be clean)
- Ensure you're on the main branch (`master`)
- Ensure you have the latest tags from remote: `git fetch --tags`
- Verify the user has npm publish permissions

If any prerequisites fail, inform the user and stop.

## 2. Identify affected packages

Run Lerna to preview which packages will be updated:

```bash
lerna changed
```

This shows packag
```

</details>
