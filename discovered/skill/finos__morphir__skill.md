---
name: finos__morphir__skill
source: https://github.com/finos/morphir/blob/108083bf9c04e6413dde9005bde8e24aa427c8fd/.claude/skills/release-manager/SKILL.md
repo: finos/morphir
kind: skill
stars: 199
last_pushed: 2026-06-10T18:49:48Z
license: apache-2.0
score: 9
domains: [devops, release-management, cli-tools]
tags: [workflow, verification, automation]
curated: 2026-06-15
curated_by: config-scout
---

# finos/morphir — skill

**Why it's worth keeping:** The inclusion of specific command sequences, a detailed task reference table, and domain-specific troubleshooting makes it an excellent template for creating 'ritual-based' agent skills.

**Summary:** A highly structured protocol for managing a full release lifecycle, covering automated verification via a task runner and manual sanity checks.

**Source credibility:** High; FinOS is a reputable financial open-source organization with active maintenance.

**Recency:** Current; utilizes modern toolchains like `mise` and follows contemporary Git/CI workflows.

**Source:** [finos/morphir/.claude/skills/release-manager/SKILL.md](https://github.com/finos/morphir/blob/108083bf9c04e6413dde9005bde8e24aa427c8fd/.claude/skills/release-manager/SKILL.md) · 199★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: release-manager
description: Assists with Morphir release management, including pre-release verification, changelog generation, and release coordination. Use when preparing releases, checking release readiness, or managing version bumps.
user-invocable: true
---

# Release Manager Skill

You are a release management assistant specialized in Morphir releases. You help ensure releases are properly verified, documented, and coordinated.

## Capabilities

1. **Pre-Release Verification** - Run all checks before releasing
2. **Changelog Management** - Generate and review changelogs
3. **Version Management** - Coordinate version bumps
4. **Release Coordination** - Manage the release workflow

## Pre-Release Verification Checklist

Before any release, run the following verification steps:

### Automated Checks

```bash
# 1. Run all formatting checks
mise run fmt-check

# 2. Run all linters
mise run lint

# 3. Run all tests
mise run test

# 4. Validate schemas against metaschema
mise run schema:validate

# 5. Validate documentation examples
mise run examples:validate

# 6. Validate fixtures
mise run fixtures:validate

# 7. Verify schema sync (YAML/JSON)
mise run docs:schema:verify
```

</details>
