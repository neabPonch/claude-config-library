---
name: crabtalk__crabtalk__0036-skill
source: https://github.com/crabtalk/crabtalk/blob/55184a0715a3dc343f6d717bff303778bca5acdf/docs/src/rfcs/0036-skill.md
repo: crabtalk/crabtalk
kind: skill
stars: 718
last_pushed: 2026-05-26T11:53:58Z
license: mit
score: 8
domains: [agents-ai, cli-tools, system-design]
tags: [skill-management, prompt-engineering, dynamic-loading]
curated: 2026-06-15
curated_by: config-scout
---

# crabtalk/crabtalk — skill

**Why it's worth keeping:** The directory-based discovery pattern with strict path traversal guards and scope-based access control provides a perfect template for building extensible agentic tools.

**Summary:** An RFC defining a robust system for discovering, dispatching, and hot-reloading agent skills stored as Markdown files.

**Source credibility:** High; the source repository is well-starred and shows recent, active development.

**Recency:** Very current/cutting-edge (includes future-dated roadmap elements).

**Source:** [crabtalk/crabtalk/docs/src/rfcs/0036-skill.md](https://github.com/crabtalk/crabtalk/blob/55184a0715a3dc343f6d717bff303778bca5acdf/docs/src/rfcs/0036-skill.md) · 718★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# 0036 - Skill Loading

- Feature Name: Skill Loading
- Start Date: 2026-03-27
- Discussion: [#36](https://github.com/crabtalk/crabtalk/issues/36)
- Crates: runtime

## Summary

How crabtalk discovers, loads, dispatches, hot-reloads, and scopes skills. The
skill format follows the [agentskills.io](https://agentskills.io) convention —
this RFC covers the loading mechanism, not the format.

## Motivation

Agents need extensible behavior without recompilation. Skills are the simplest
unit that works: a markdown file with a name, description, and a prompt body.
No code generation, no plugin API, no runtime linking.

The format is defined by [agentskills.io](https://agentskills.io). What crabtalk
needs to decide is how skills are found on disk, how they're resolved at
runtime, how they stay current without restarts, and how agents are restricted
to subsets of available skills.

## Design

### Format

SKILL.md follows the [agentskills.io](https://agentskills.io) convention.
Required fields: `name`, `description`. Optional: `allowed-tools`. The markdown
body is the skill prompt.

### Discovery

`SkillHandler::load(dirs)` scans a list of directories (in config-defined order)
recursively fo
```

</details>
