---
name: grafana__tempo__skill
source: https://github.com/grafana/tempo/blob/48c5a466e031ca86ab920979caee194a7549bb2d/.claude/skills/fix-vendor-conflicts/SKILL.md
repo: grafana/tempo
kind: skill
stars: 5307
last_pushed: 2026-06-15T08:03:31Z
license: agpl-3.0
score: 9
domains: [backend, go-development]
tags: [golang, vendoring, git-workflow]
curated: 2026-06-15
curated_by: config-scout
---

# grafana/tempo — skill

**Why it's worth keeping:** Provides specific verification commands (like `go test -run ^$` to catch test-file compile errors) and strategic heuristics for choosing between cherry-picking and manual patching.

**Summary:** A rigorous procedural skill for resolving Go module and vendor conflicts by leveraging the main branch as a ground truth.

**Source credibility:** Highly credible; sourced from Grafana Tempo, a highly-regarded production tracing backend.

**Recency:** Current; utilizes modern Go toolchain practices compatible with recent Claude Code capabilities.

**Source:** [grafana/tempo/.claude/skills/fix-vendor-conflicts/SKILL.md](https://github.com/grafana/tempo/blob/48c5a466e031ca86ab920979caee194a7549bb2d/.claude/skills/fix-vendor-conflicts/SKILL.md) · 5307★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: fix-vendor-conflicts
description: Resolve vendor/ conflicts during a merge, rebase, or dependency upgrade on main or release branches
allowed-tools: Bash Read Grep Edit
---

# Fixing Vendor Conflicts

Use this skill when resolving conflicts in `vendor/` during a merge, rebase, or dependency upgrade.

## Before starting

**Ask the user:** are you working on the **main** branch or a **release** branch? The answer changes what kinds of fixes are acceptable (see below).

## What this skill does

Guides the process of diagnosing and resolving vendor directory conflicts caused by dependency changes — whether a direct bump or a transitive cascade.

---

## Core principles

**Never patch vendor/ files manually.** CI runs `go mod vendor` and will overwrite any manual patches. All fixes must come from upgrading or pinning the upstream dependency to a version that has the fix already.

**Always run the pre-commit checklist before committing anything:**

```bash
go mod tidy
go mod vendor
go build -mod vendor ./...
go test -mod vendor -run ^$ ./...
go run pkg/docsgen/generate_manifest.go
```

All must pass with no errors. If `generate_manifest.go` produces changes, commit them:

```ba
```

</details>
