---
name: ibrahimk2002__job-match-agent__axis-measure-skill
source: https://github.com/ibrahimk2002/job-match-agent/blob/2d7896472b29702b64f8ffe972e88df52214fea7/docs/AXIS_MEASURE_SKILL.md
repo: ibrahimk2002/job-match-agent
kind: skill
stars: 0
last_pushed: 2026-06-15T16:13:22Z
license: unknown
score: 9
domains: [data-extraction, software-engineering]
tags: [scoring-engine, structured-output]
curated: 2026-06-16
curated_by: config-scout
---

# ibrahimk2002/job-match-agent — skill

**Why it's worth keeping:** Uses sophisticated prompting techniques like signal-source weighting and a mathematical formula for derived metrics to ensure data consistency.

**Summary:** A specialized skill that parses job descriptions into weighted competency vectors across seven technical axes.

**Source credibility:** Low social proof (0 stars), but the underlying logic demonstrates expert-level prompt engineering architecture.

**Recency:** Current; uses modern tech stacks and follows advanced agentic reasoning patterns.

**Source:** [ibrahimk2002/job-match-agent/docs/AXIS_MEASURE_SKILL.md](https://github.com/ibrahimk2002/job-match-agent/blob/2d7896472b29702b64f8ffe972e88df52214fea7/docs/AXIS_MEASURE_SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: jd-competency-scorer
description: Score software engineering job descriptions on a fixed set of competency axes to produce a weighted skill distribution profile of the ideal candidate. Use this skill whenever a user pastes a job description, job posting, or role spec and asks to profile it, rank the skills it emphasizes, compare it against other roles, produce a competency vector, assess candidate fit, or weight required skills — even if they don't use the word "score." Also trigger for requests like "what kind of engineer does this role want," "break down this JD by skill area," or when multiple JDs are provided for comparison.
---

> **⚠ Sync note:** This document is the source of truth for axis names,
> definitions, scoring philosophy, and calibration. Its body is embedded
> verbatim into `src/prompts/extraction.txt`. **When you edit this file,
> update `extraction.txt` and bump its `# prompt_version:` line.**

# JD Competency Scorer

## What this skill does

Given one or more software engineering job descriptions, produce a JSON object scoring the role on 7 competency axes. Each score is a float in `[0.0, 1.0]` representing how central that competency is to the ideal
```

</details>
