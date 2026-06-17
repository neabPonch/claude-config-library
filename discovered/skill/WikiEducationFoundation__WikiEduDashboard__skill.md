---
name: WikiEducationFoundation__WikiEduDashboard__skill
source: https://github.com/WikiEducationFoundation/WikiEduDashboard/blob/24e403fb086cacee0a46f8ebc93c943200b3c0a0/.claude/skills/course-update-recon/SKILL.md
repo: WikiEducationFoundation/WikiEduDashboard
kind: skill
stars: 429
last_pushed: 2026-06-15T18:18:14Z
license: mit
score: 9
domains: [backend-api, cli-tools, observability]
tags: [diagnostics, performance-tuning, reconnaissance]
curated: 2026-06-15
curated_by: config-scout
---

# WikiEducationFoundation/WikiEduDashboard — skill

**Why it's worth keeping:** It enforces strict safety boundaries (no SSH) and uses a mathematical projection model to distinguish between scale problems and service-level bottlenecks.

**Summary:** A diagnostic workflow to characterize slow course updates by estimating workload via public JSON endpoints and benchmarked cost axes.

**Source credibility:** Highly credible; high star count and very recent commits from the Wiki Education Foundation.

**Recency:** Extremely current, referencing specific future-dated benchmark documentation (2026).

**Source:** [WikiEducationFoundation/WikiEduDashboard/.claude/skills/course-update-recon/SKILL.md](https://github.com/WikiEducationFoundation/WikiEduDashboard/blob/24e403fb086cacee0a46f8ebc93c943200b3c0a0/.claude/skills/course-update-recon/SKILL.md) · 429★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: course-update-recon
description: Characterize a slow / stuck course-update worker on dashboard.wikiedu.org or outreachdashboard.wmflabs.org. Use this skill when asked to investigate why a course update is taking unusually long, hung, or running for many hours, or to estimate the scale-of-work of an in-flight update. Pure HTTP recon against public APIs — never SSH into prod.
---

# Course-update recon

Workflow for characterizing a slow or stuck course update without ever
touching prod. The goal is a per-axis estimate of the work-in-flight
(or work-just-completed) so we can predict runtime and pick a fix.

**Hard rule: never SSH to peony-web, peony-database, peony-sidekiq*,
dashboard.wikiedu.org, or any other prod host.** All recon is via
public dashboard JSON endpoints + public Wikimedia APIs. If you need
something only available inside the prod app, ask the user to run a
one-liner and paste the result back.

## Step 1 — Resolve course id → slug

The numeric id is what the user usually has; the public JSON endpoints
key on slug. The `/find_course/<id>` endpoint redirects from id to the
canonical course URL — read the `Location:` header to get the slug:

```bash
curl -sSI
```

</details>
