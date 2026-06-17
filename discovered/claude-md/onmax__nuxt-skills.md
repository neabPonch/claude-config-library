---
name: onmax__nuxt-skills
source: https://github.com/onmax/nuxt-skills/blob/311074589914796ad39356bf42ab68f920ebee04/CLAUDE.md
repo: onmax/nuxt-skills
kind: claude-md
stars: 682
last_pushed: 2026-06-01T07:41:14Z
license: unknown
score: 8
domains: [agents-ai, documentation-engineering]
tags: [meta-instructions, manifest-management, context-optimization]
curated: 2026-06-16
curated_by: config-scout
---

# onmax/nuxt-skills — claude-md

**Why it's worth keeping:** Uses mandatory checklists to ensure multi-file consistency (JSON manifests + Markdown) and defines a 'progressive loading' pattern to optimize context window efficiency.

**Summary:** Provides strict operational protocols for maintaining a skill-based documentation repository used by AI agents.

**Source credibility:** High; highly starred repo with active, recent maintenance.

**Recency:** Very current, specifically tailored for Nuxt 4+ and modern Claude Code workflows.

**Source:** [onmax/nuxt-skills/CLAUDE.md](https://github.com/onmax/nuxt-skills/blob/311074589914796ad39356bf42ab68f920ebee04/CLAUDE.md) · 682★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Purpose

Claude Code skills for Vue 3, Nuxt 4+, NuxtHub v0.10, and Nuxt module development. Pure documentation repo - no build/test commands.

## Structure

Follows [agentskills](https://github.com/agentskills/agentskills) standard format.

- `skills/<name>/SKILL.md` - Entry point (frontmatter with name/description/license)
- `skills/<name>/references/*.md` - Sub-files loaded on-demand
- `.claude-plugin/plugin.json` - Claude Code plugin manifest
- `.claude-plugin/marketplace.json` - Claude Code marketplace manifest

## MANDATORY: Before Starting Work

**Always run `git pull`** before making any changes. CI auto-commits lint fixes, so your local branch may be behind.

**After making changes, sync to `~/.claude/skills/`** by running `./sync-skills.sh` so Claude Code uses latest versions.

## MANDATORY: When Working on Skills

**Always use the `example-skills:skill-creator` skill** when creating or editing any skill content. This ensures skills follow best practices.

### Checklist When Changing Skills

When adding/editing/removing a skill, update ALL of these:

1. `
```

</details>
