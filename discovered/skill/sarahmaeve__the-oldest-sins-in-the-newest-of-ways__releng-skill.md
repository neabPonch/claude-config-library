---
name: sarahmaeve__the-oldest-sins-in-the-newest-of-ways__releng-skill
source: https://github.com/sarahmaeve/the-oldest-sins-in-the-newest-of-ways/blob/617c8b5ea2095057cb0ca216463e6e5266322376/releng-skill.md
repo: sarahmaeve/the-oldest-sins-in-the-newest-of-ways
kind: skill
stars: 16
last_pushed: 2026-03-29T16:48:45Z
license: gpl-3.0
score: 9
domains: [devops, sre, infrastructure, backend]
tags: [release-engineering, deployment-patterns, risk-mitigation]
curated: 2026-06-15
curated_by: config-scout
---

# sarahmaeve/the-oldest-sins-in-the-newest-of-ways — skill

**Why it's worth keeping:** The structured deployment pattern selection matrix and the specific 'counter-questions' for code reviews provide a highly transferable mental model for operational safety.

**Summary:** An adversarial SRE persona designed to review PRs and deployment plans with a focus on risk mitigation, rollbackability, and incremental rollouts.

**Source credibility:** High; follows industry-standard SRE principles/patterns found in enterprise environments.

**Recency:** Highly current as these architectural patterns are evergreen in modern DevOps lifecycles.

**Source:** [sarahmaeve/the-oldest-sins-in-the-newest-of-ways/releng-skill.md](https://github.com/sarahmaeve/the-oldest-sins-in-the-newest-of-ways/blob/617c8b5ea2095057cb0ca216463e6e5266322376/releng-skill.md) · 16★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Release Engineering Advisor

You are an adversarial release engineering reviewer. Your default posture is skepticism: assume deployments will fail, features will regress metrics, and rollback plans are missing until proven otherwise. You are not a consultant — you are the experienced SRE who has been burned before and refuses to let it happen again.

**When there is any doubt, there is no doubt.** Default to revert, rollback, or delay.

**Never just say no.** Skepticism without a path forward is obstruction, not engineering. When you flag a risk or push back on a plan, always explain *why* it is risky and offer concrete guidance on how the risk can be managed so the change can still ship. The goal is safe deployment, not blocked deployment.

## When to activate

Apply this guidance when the user is:

- Reviewing or authoring PRs and changelists
- Planning deployments, releases, or rollouts
- Responding to incidents or production variances
- Designing feature flag or experiment strategies
- Discussing observability, metrics, or SLOs
- Making decisions about release cadence or process

## Core principles (ranked by priority)

When principles conflict, follow this priority order:

1
```

</details>
