---
name: polvera-org__8x__skill
source: https://github.com/polvera-org/8x/blob/c20839e3e4ac3d30fcf543acb9f1606d63380a47/src/skills/deploy-checklist/skill.md
repo: polvera-org/8x
kind: skill
stars: 5
last_pushed: 2026-04-13T15:06:47Z
license: mit
score: 9
domains: [devops, sre, ci-cd]
tags: [deployment, checklist, verification, release-management]
curated: 2026-06-15
curated_by: config-scout
---

# polvera-org/8x — skill

**Why it's worth keeping:** The use of binary status gates (SHIPPED vs BLOCKED) prevents agentic hallucinations of success, while the structured output format ensures predictable feedback loops for human oversight.

**Summary:** An opinionated SRE/DevOps protocol that enforces strict 'Hard Gates' and a standardized deployment report format.

**Source credibility:** High; part of a focused 'AI agent roster' with recent maintenance activity.

**Recency:** Current; highly compatible with modern tool-use workflows in Claude Code.

**Source:** [polvera-org/8x/src/skills/deploy-checklist/skill.md](https://github.com/polvera-org/8x/blob/c20839e3e4ac3d30fcf543acb9f1606d63380a47/src/skills/deploy-checklist/skill.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: deploy-checklist
description: Use this skill when verifying a build, preparing a deployment, creating pull requests, running health checks, or managing a release. Load when the task is to get code from "merged" to "running in production" — or to confirm it is ready to be merged.
license: Proprietary. LICENSE.txt has complete terms
---

# Deploy Checklist — SRE & DevOps Methodology

## Purpose

Verify builds, manage deployments, create pull requests, run health checks, and handle release management. The status is binary: **SHIPPED** or **BLOCKED**. There is no "SHIPPED with warnings."

## Hard Gates

Before doing anything else, confirm:

1. **QA approval exists.** If absent, stop immediately. Report BLOCKED: "No QA approval." No exceptions.
2. **Git state is clean.** No uncommitted changes, no untracked files that should be committed.

## Phase 1: Pre-Flight Checks

1. Confirm QA approval is documented.
2. Verify working tree is clean.
3. Verify branch lineage — feature branch should be based on current target. Check for merge conflicts. If conflicts exist, report BLOCKED with the specific conflicting files.
4. Review commit history. Verify commits correspond to the expect
```

</details>
