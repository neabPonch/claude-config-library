---
name: mono__SkiaSharp__skill
source: https://github.com/mono/SkiaSharp/blob/e3bca18bffbc55db3655d623bb32f8935f22726f/.agents/skills/issue-triage/SKILL.md
repo: mono/SkiaSharp
kind: skill
stars: 5439
last_pushed: 2026-06-15T09:44:44Z
license: mit
score: 9
domains: [cli-tools, devops, automation]
tags: [triage, github-workflow, structured-output]
curated: 2026-06-15
curated_by: config-scout
---

# mono/SkiaSharp — skill

**Why it's worth keeping:** It uses 'mandatory first steps' to force the agent to read schema/anti-patterns, reducing hallucinations; the phased approach (Investigate -> Analyze -> Validate) is a perfect template for any maintenance task.

**Summary:** A highly sophisticated, multi-phase investigative pipeline that enforces strict schema compliance and source-code verification before classification.

**Source credibility:** Very high; SkiaSharp is a major, industry-standard graphics library with active maintenance.

**Recency:** Current; uses modern tool patterns like the GitHub CLI and structured JSON schema enforcement.

**Source:** [mono/SkiaSharp/.agents/skills/issue-triage/SKILL.md](https://github.com/mono/SkiaSharp/blob/e3bca18bffbc55db3655d623bb32f8935f22726f/.agents/skills/issue-triage/SKILL.md) · 5439★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: issue-triage
description: >-
  Triage a SkiaSharp GitHub issue or PR into structured JSON with classification
  (type, area, platform, severity), suggested response, automatable actions, and
  companion Markdown/HTML reports. Triggers: "triage #123", "triage issue",
  "classify issue", "analyze issue", "what's this issue about". Also triggered
  when an issue number is given after the issue-triage skill is already mentioned.
---

# Triage Issue

**Issue pipeline: Step 1 of 3 (Triage).** See [`documentation/dev/issue-pipeline.md`](../../../documentation/dev/issue-pipeline.md).

Analyze a SkiaSharp GitHub issue and produce a structured, schema-validated triage JSON.

## ⛔ MANDATORY FIRST STEPS (do not skip)

1. Read THIS entire SKILL.md before any investigation
2. Read [references/schema-cheatsheet.md](references/schema-cheatsheet.md) for required fields and enums
3. Read [references/anti-patterns.md](references/anti-patterns.md) for critical rules

These 3 reads are REQUIRED. Do not proceed to Phase 1 until all three are loaded.

> **Quick flow:**
> 1. Load issue data from GitHub (prefer `gh`, or GitHub MCP when available)
> 2. Read references: [schema-cheatsheet](referenc
```

</details>
