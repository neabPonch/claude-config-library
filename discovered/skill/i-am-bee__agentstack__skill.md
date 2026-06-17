---
name: i-am-bee__agentstack__skill
source: https://github.com/i-am-bee/agentstack/blob/79c786049d39684841d77fef9abfd8457a58b0bf/.claude/skills/release-notes/SKILL.md
repo: i-am-bee/agentstack
kind: skill
stars: 1122
last_pushed: 2026-06-08T18:15:43Z
license: apache-2.0
score: 9
domains: [devops, documentation, cli-tools, git-workflow]
tags: [release-notes, github-integration, automation, persona-based]
curated: 2026-06-15
curated_by: config-scout
---

# i-am-bee/agentstack — skill

**Why it's worth keeping:** Demonstrates a sophisticated 'search-then-synthesize' pattern using the `gh` CLI; provides clear persona-based instructions to prevent generic technical listings.

**Summary:** Automates release note generation by calculating version diffs via shell scripts and extracting deep context from GitHub PR comments. It translates technical changes into impact-driven narratives tailored to specific user personas.

**Source credibility:** High; repository has significant stars and shows active maintenance/recent activity.

**Recency:** Current; utilizes modern GitHub CLI workflows highly compatible with Claude Code shell capabilities.

**Source:** [i-am-bee/agentstack/.claude/skills/release-notes/SKILL.md](https://github.com/i-am-bee/agentstack/blob/79c786049d39684841d77fef9abfd8457a58b0bf/.claude/skills/release-notes/SKILL.md) · 1122★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: release-notes
description: Helps generate release notes to be published on GitHub as well as in a Slack community channel
---

When tasked to generate release notes for a given version, your goal is to produce good-quality release notes focused on the user of Agent Stack. You don't need to provide a list of changed tickets or merged PRs; your goal is to provide human-readable release notes focused on the impact on the user.

## Scope of the release

The user generally provides a version tag for which they want to generate release notes. For example, they might tell you something like "Generate release notes for release-v0.5.0". Your first task is to figure out what the scope of the release is. The scope is basically a list of all merged PRs; once you have this list, you can proceed to the next steps.

### How to figure out the scope of the release

The user tells you for which version they want to generate the release notes, e.g., `release-v0.5.0`. Your next step is to figure out what the start commit in the git history is, and then you compare that with the head of the given release, e.g., `release-v0.5.0`.

The start commit is the latest stable version of the Agent Stac
```

</details>
