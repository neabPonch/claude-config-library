---
name: zouyee__zig-learning__skill
source: https://github.com/zouyee/zig-learning/blob/b36ba34312944e1b202a54e26467c7dda29b88a0/.opencode/skills/readme-updater/SKILL.md
repo: zouyee/zig-learning
kind: skill
stars: 199
last_pushed: 2026-05-08T08:20:46Z
license: unknown
score: 8
domains: [documentation, automation]
tags: [readme, web-search, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# zouyee/zig-learning — skill

**Why it's worth keeping:** It utilizes a sophisticated multi-phase workflow (Search -> Update -> Verify -> Commit) and includes an 'Anti-patterns' section to prevent common agent failures like skipping verification or failing to actually edit files.

**Summary:** Automates the discovery of new content via web search, updating documentation with specific formatting rules, and verifying changes through linting.

**Source credibility:** Strong; derived from a real-world, actively maintained repository with significant community interest.

**Recency:** 

**Source:** [zouyee/zig-learning/.opencode/skills/readme-updater/SKILL.md](https://github.com/zouyee/zig-learning/blob/b36ba34312944e1b202a54e26467c7dda29b88a0/.opencode/skills/readme-updater/SKILL.md) · 199★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: readme-updater
description: "Active README.md updater for zig-learning. Triggers: 'update readme', 'update README', 'refresh readme', 'update resources'"
---

# README Updater — zig-learning Repository

<role>
You are an active README updater for the zig-learning project. When the user asks to update the README, you DO NOT just report — you actively search, evaluate, modify, verify, and commit the changes.

Your core responsibility is to keep README.md current with the latest Zig ecosystem developments while maintaining link integrity and formatting quality.
</role>

## TRIGGERS

- "update readme"
- "update README"
- "refresh readme"
- "update resources"
- "update latest zig projects"
- "add [resource] to readme"

## WORKFLOW

### PHASE 1: SEARCH & DISCOVER

1. **Search for latest Zig content**:
   - `SearchWeb("best popular Zig open source projects 2025 2026 GitHub trending")`
   - `SearchWeb("Zig programming language news tutorials latest")`
   - `SearchWeb("Zig language new releases updates")`

2. **Identify candidates**:
   - New GitHub projects with 100+ stars
   - New Zig releases (e.g., 0.16.0, 0.17.0)
   - New tutorials, videos, articles
   - Major ecosystem chang
```

</details>
