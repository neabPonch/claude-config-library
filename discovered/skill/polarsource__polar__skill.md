---
name: polarsource__polar__skill
source: https://github.com/polarsource/polar/blob/94b7ac96b500c22d42a3e01bf5e80cd90667b6de/.agents/skills/fix-sentry/SKILL.md
repo: polarsource/polar
kind: skill
stars: 9940
last_pushed: 2026-06-15T08:38:43Z
license: apache-2.0
score: 8
domains: [backend, observability, devops]
tags: [sentry, debugging, git-worktrees, error-resolution]
curated: 2026-06-15
curated_by: config-scout
---

# polarsource/polar — skill

**Why it's worth keeping:** It demonstrates how to use unique identifiers (correlation IDs) to bridge disparate data sources and enforces a professional git worktree pattern for safe, isolated development.

**Summary:** Automates debugging by correlating Sentry error reports with observability logs and guiding the agent through a structured fix-and-PR workflow.

**Source credibility:** Highly credible; based on a highly-starred, actively maintained open-source repository.

**Recency:** Current; follows modern agentic tool-use patterns.

**Source:** [polarsource/polar/.agents/skills/fix-sentry/SKILL.md](https://github.com/polarsource/polar/blob/94b7ac96b500c22d42a3e01bf5e80cd90667b6de/.agents/skills/fix-sentry/SKILL.md) · 9940★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: fix-sentry
description: Analyze and fix issues reported by Sentry in the Polar codebase.
user-invocable: true
allowed-tools: Bash(gh:*) Bash(git:*) logfire_polar* sentry_polar* github*
---

You're responsible for analyzing and fixing issues reported by Sentry in the Polar codebase. This involves investigating the Sentry reports, identifying the root causes of the issues, and implementing fixes to resolve them.

## Input

If not provided in the invocation prompt, you should ask the user for the a Sentry issue ID or a link to the Sentry issue. This will allow you to access the details of the issue and begin your analysis.

The Sentry organization ID of Polar is `4505046560538624` and its slug is `polar-sh`.

## Step 1: Analyze the Sentry issue

Using the sentry_polar tools, access the details of the Sentry issue provided by the user. This includes the error message, stack trace, and any additional context or metadata associated with the issue.

## Step 2: correlate with Logfire logs

Extract the `correlation_id` tag from the Sentry issue. If available, use it to search for related logs in Logfire using the logfire_polar tools. This can provide additional context and insight
```

</details>
