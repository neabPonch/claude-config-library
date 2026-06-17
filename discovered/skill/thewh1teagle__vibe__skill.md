---
name: thewh1teagle__vibe__skill
source: https://github.com/thewh1teagle/vibe/blob/e1dd7c942a770e0bea26d302f058ed8455a94dff/.skills/aptabase-analytics-report/SKILL.md
repo: thewh1teagle/vibe
kind: skill
stars: 6449
last_pushed: 2026-05-01T16:12:39Z
license: mit
score: 9
domains: [data-analysis, reliability-engineering]
tags: [analytics, telemetry, python, reporting]
curated: 2026-06-15
curated_by: config-scout
---

# thewh1teagle/vibe — skill

**Why it's worth keeping:** Demonstrates an elite pattern of using 'ad-hoc' scripting (via uv + inline Python) to prevent script staleness, while providing a strict 'Done Checklist' to ensure analytical completeness.

**Summary:** Provides a structured workflow for exporting telemetry data and performing ad-hoc statistical analysis via inline Python/Pandas. It transforms raw event logs into actionable reliability reports tied to specific code paths.

**Source credibility:** High; the source repository is highly starred and actively maintained.

**Recency:** 

**Source:** [thewh1teagle/vibe/.skills/aptabase-analytics-report/SKILL.md](https://github.com/thewh1teagle/vibe/blob/e1dd7c942a770e0bea26d302f058ed8455a94dff/.skills/aptabase-analytics-report/SKILL.md) · 6449★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: aptabase-analytics-report
description: Export and analyze Vibe Aptabase analytics for recent time windows or existing CSV exports, with emphasis on failure rates, affected users, app versions, and OS breakdowns. Use when Codex needs to: (1) export recent analytics with `scripts/export_analytics.py`, (2) filter an export to the exact last N hours, (3) restrict analysis to specific `app_version` values, (4) quantify the impact of the current failure-related events defined in the repository, or (5) produce a concise reliability report with fix suggestions.
---

# Aptabase Analytics Report

## Overview

Use this skill to export Aptabase telemetry from the Vibe repo, trim day-granularity exports to an exact time window, and produce a reliability report from the CSV with inline `uv` + pandas commands.

## Prerequisites

The export script requires a `.env` file at the repo root with these variables:

- `BASE_URL` – Aptabase server URL
- `AUTH_SECRET` – JWT signing secret
- `AUTH_NAME` – account name
- `AUTH_EMAIL` – account email
- `APP_KEY` – app key (e.g. `A-SH-0194598703`)
- `APTABASE_REGION` – optional, defaults to `"SH"`

## CSV Schema

The exported CSV contains these colum
```

</details>
