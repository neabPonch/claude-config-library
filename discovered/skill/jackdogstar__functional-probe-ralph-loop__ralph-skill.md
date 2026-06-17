---
name: jackdogstar__functional-probe-ralph-loop__ralph-skill
source: https://github.com/jackdogstar/functional-probe-ralph-loop/blob/12bef904e2015d3eb91bfe11c9607a7232eafb9d/ralph-skill.md
repo: jackdogstar/functional-probe-ralph-loop
kind: skill
stars: 0
last_pushed: 2026-02-03T19:08:15Z
license: unknown
score: 8
domains: [agents-ai, software-engineering]
tags: [autonomous-loop, state-tracking, scaffolding]
curated: 2026-06-15
curated_by: config-scout
---

# jackdogstar/functional-probe-ralph-loop — skill

**Why it's worth keeping:** It utilizes `prd.json` to maintain structured execution state and `AGENTS.md` to prevent context drift during long-running tasks. The 'spec-driven' approach forces mandatory validation for every incremental unit of work.

**Summary:** Defines a methodology for creating an autonomous, self-validating development loop that decomposes projects into granular, testable stories. It organizes work through domain-specific spec files, state tracking via JSON, and a central agent manual.

**Source credibility:** Low social proof on GitHub, but the structural depth indicates a high level of prompt engineering expertise.

**Recency:** Current; aligns with contemporary agentic loop and state-management paradigms.

**Source:** [jackdogstar/functional-probe-ralph-loop/ralph-skill.md](https://github.com/jackdogstar/functional-probe-ralph-loop/blob/12bef904e2015d3eb91bfe11c9607a7232eafb9d/ralph-skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Ralph Wiggums Loop — Project Generation Skill

## Purpose

This skill instructs Claude on how to generate a complete, runnable **Ralph Wiggums Loop** project from any functional specification. A Ralph Loop is an autonomous AI-driven development system that uses Claude to iteratively plan and build a software project, story by story, with full validation at every step.

---

## What You Will Produce

Given a functional specification, generate the following directory structure:

```
<project-name>-ralph/
├── loop.sh                          # Main autonomous loop script
├── prd.json                         # Product Requirements Document (all user stories)
├── AGENTS.md                        # Agent operations manual for Claude
├── PROMPT_plan.md                   # Planning mode prompt
├── PROMPT_build.md                  # Building mode prompt
├── <functional-spec-filename>.md    # Copy of the provided functional specification
└── specs/                           # Numbered spec files, one per domain area
    ├── 01-<first-area>.md
    ├── 02-<second-area>.md
    └── ...
```

---

## Step-by-Step Generation Process

### Step 1: Analyze the Functional Specification

Read the enti
```

</details>
