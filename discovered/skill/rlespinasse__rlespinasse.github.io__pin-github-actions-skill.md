---
name: rlespinasse__rlespinasse.github.io__pin-github-actions-skill
source: https://github.com/rlespinasse/rlespinasse.github.io/blob/c0e67e557c3600f8da57e881653bd5de7f202fbe/content/posts/pin-github-actions-skill.md
repo: rlespinasse/rlespinasse.github.io
kind: skill
stars: 1
last_pushed: 2026-06-15T12:41:26Z
license: mit
score: 9
domains: [security, ci-cd, devops, github-actions]
tags: [sha-pinning, automation, dependabot, supply-chain-security]
curated: 2026-06-16
curated_by: config-scout
---

# rlespinasse/rlespinasse.github.io — skill

**Why it's worth keeping:** It implements a sophisticated multi-step workflow (Discovery -> Resolution via API -> Replacement -> Configuration) including safety logic for major version jumps. The inclusion of automated maintenance/Dependabot setup is an excellent pattern for high-quality agentic tasks.

**Summary:** Automates the migration of GitHub Actions from tag references to exact commit SHAs for improved supply chain security. It also configures Dependabot with grouped updates to prevent future maintenance burdens.

**Source credibility:** High; highly specific technical skill with clear, structured execution steps.

**Recency:** Extremely current (dated 2026), reflecting modern security best practices.

**Source:** [rlespinasse/rlespinasse.github.io/content/posts/pin-github-actions-skill.md](https://github.com/rlespinasse/rlespinasse.github.io/blob/c0e67e557c3600f8da57e881653bd5de7f202fbe/content/posts/pin-github-actions-skill.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
title: "Pin GitHub Actions Skill: Automating SHA Pinning with AI Assistants"
date: 2026-03-15T13:00:00+01:00
draft: false
summary: "The pin-github-actions skill automates SHA pinning of GitHub Actions, handling API lookups, tag dereferencing, and Dependabot setup."
featureimage: /img/posts/pin-github-actions-skill/featured.svg
tags:
- opensource
- github
- ci/cd
- security
- ai
categories:
- Technical posts
- Open Source
series: ["AI Skills"]
series_order: 4
---

SHA pinning GitHub Actions is a [well-understood security practice](/posts/github-actions-commit-sha-pinning/).
Replacing `actions/checkout@v4` with a full commit SHA prevents a compromised tag from silently changing the code your CI runs.

The problem is not understanding why to do it.
The problem is doing it.

A typical migration means: enumerate every `uses:` reference across all workflow files, look up the latest release for each action, resolve the commit SHA (handling annotated tags that need dereferencing), replace every reference, add version comments, and then configure Dependabot so the SHAs stay current.
For a repository with three workflows and six different actions, this is already tedious.
For an organisa
```

</details>
