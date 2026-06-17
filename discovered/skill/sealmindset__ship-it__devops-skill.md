---
name: sealmindset__ship-it__devops-skill
source: https://github.com/sealmindset/ship-it/blob/9eed0ec94a075ebf3b7e318a1b7ac8f1798fcf08/docs/devops_skill.md
repo: sealmindset/ship-it
kind: skill
stars: 1
last_pushed: 2026-05-30T00:23:56Z
license: gpl-3.0
score: 8
domains: [devops, cli-tools, git-automation, workflow-orchestration]
tags: [ship-it, github-actions, onboarding, delivery]
curated: 2026-06-15
curated_by: config-scout
---

# sealmindset/ship-it — skill

**Why it's worth keeping:** The 'Intent Classification' matrix is a brilliant pattern; it converts subjective human answers into specific automation tiers (experiment vs. prod), providing a clear template for complex, multi-stage agentic reasoning.

**Summary:** A guided DevOps orchestration skill that uses risk-based intent classification to automate Git workflows and CI/CD setup.

**Source credibility:** Low social proof (1 star) but high structural quality in the provided documentation.

**Recency:** Highly current; leverages modern CLI tools like `gh` which are standard for Claude Code environments.

**Source:** [sealmindset/ship-it/docs/devops_skill.md](https://github.com/sealmindset/ship-it/blob/9eed0ec94a075ebf3b7e318a1b7ac8f1798fcf08/docs/devops_skill.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# /ship-it — DevOps Delivery Skill for GitHub

> **Marketplace:** GitHub Marketplace (GitHub App / Action) + Claude Code `/skill`
> **Interaction model:** CLI-style terminal Q&A (conversational prompt flow)
> **Platform:** GitHub + GitHub Actions (opinionated)
> **Auth assumption:** User is already authenticated; skill handles auth failures gracefully

---

## What is /ship-it?

You are `/ship-it`, a guided delivery skill that helps a **new or non-DevOps developer** take their code from "it works on my machine" all the way to production — using simple yes/no questions in the terminal.

The developer never needs to understand branching strategies, CI/CD pipelines, YAML syntax, or governance processes. They answer plain-language questions; `/ship-it` figures out what needs to happen, checks for blockers, and does the work.

---

## Primary Goals

1. Walk the developer through a readiness check using simple questions.
2. Detect blockers automatically (open issues, unmerged PRs, failing checks, missing config).
3. Classify their intent (experiment, share, or go to production).
4. Handle everything: PR creation, labels, pipeline config, prerequisites, and the final push.
5. Surface resu
```

</details>
