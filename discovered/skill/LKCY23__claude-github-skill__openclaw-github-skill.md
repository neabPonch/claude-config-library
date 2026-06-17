---
name: LKCY23__claude-github-skill__openclaw-github-skill
source: https://github.com/LKCY23/claude-github-skill/blob/8ba6659ae35d73a0a9fe09ffcc07464e5169668e/openclaw-github-SKILL.md
repo: LKCY23/claude-github-skill
kind: skill
stars: 0
last_pushed: 2026-03-25T04:06:55Z
license: unknown
score: 8
domains: [cli-tools, devops, github]
tags: [github, gh-cli, automation]
curated: 2026-06-16
curated_by: config-scout
---

# LKCY23/claude-github-skill — skill

**Why it's worth keeping:** Includes essential 'When NOT to use' guardrails and advanced '--json' + 'jq' patterns that allow an agent to parse structured data reliably.

**Summary:** Provides structured instructions for using the GitHub CLI (gh) to manage PRs, issues, and CI/CD workflows.

**Source credibility:** Low social proof (0 stars), but high technical quality in the command examples.

**Recency:** Current; follows modern GitHub CLI usage patterns.

**Source:** [LKCY23/claude-github-skill/openclaw-github-SKILL.md](https://github.com/LKCY23/claude-github-skill/blob/8ba6659ae35d73a0a9fe09ffcc07464e5169668e/openclaw-github-SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: github
description: "GitHub operations via `gh` CLI: issues, PRs, CI runs, code review, API queries. Use when: (1) checking PR status or CI, (2) creating/commenting on issues, (3) listing/filtering PRs or issues, (4) viewing run logs. NOT for: complex web UI interactions requiring manual browser flows (use browser tooling when available), bulk operations across many repos (script with gh api), or when gh auth is not configured."
metadata:
  {
    "openclaw":
      {
        "emoji": "🐙",
        "requires": { "bins": ["gh"] },
        "install":
          [
            {
              "id": "brew",
              "kind": "brew",
              "formula": "gh",
              "bins": ["gh"],
              "label": "Install GitHub CLI (brew)",
            },
            {
              "id": "apt",
              "kind": "apt",
              "package": "gh",
              "bins": ["gh"],
              "label": "Install GitHub CLI (apt)",
            },
          ],
      },
  }
---

# GitHub Skill

Use the `gh` CLI to interact with GitHub repositories, issues, PRs, and CI.

## When to Use

✅ **USE this skill when:**

- Checking PR status, reviews, or merge readiness
- Viewing C
```

</details>
