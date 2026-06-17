---
name: tis-abe-akira__pairwise-skill__skill
source: https://github.com/tis-abe-akira/pairwise-skill/blob/6110431097937a739e40056b9ffff72f9e1ec994/.claude/skills/pairwise-tester/skill.md
repo: tis-abe-akira/pairwise-skill
kind: skill
stars: 0
last_pushed: 2025-12-17T12:15:40Z
license: unknown
score: 7
domains: [testing, java, qa]
tags: [pairwise, junit, combinatorial-testing]
curated: 2026-06-15
curated_by: config-scout
---

# tis-abe-akira/pairwise-skill — skill

**Why it's worth keeping:** It defines a clear division of labor between deterministic script-based data generation and LLM-led business logic implementation via TODO markers.

**Summary:** Provides a structured workflow for generating combinatorial JUnit test cases using a specific Java DSL and all-pairs algorithm.

**Source credibility:** Low (0 stars, unknown license).

**Recency:** Current with modern Java testing patterns.

**Source:** [tis-abe-akira/pairwise-skill/.claude/skills/pairwise-tester/skill.md](https://github.com/tis-abe-akira/pairwise-skill/blob/6110431097937a739e40056b9ffff72f9e1ec994/.claude/skills/pairwise-tester/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
skill: pairwise-tester
description: Generate JUnit test cases using Pairwise (All-Pairs) testing method to reduce combinatorial explosion while maintaining coverage
tags: [testing, pairwise, junit, combinatorial]
---

# Pairwise Test Generator Skill

This skill generates JUnit test cases using the Pairwise (All-Pairs) testing technique.

## What is Pairwise Testing?

Pairwise testing reduces the number of test cases needed when testing combinations of multiple parameters. Instead of testing all possible combinations (which can be millions), pairwise testing ensures that every pair of parameter values is tested at least once.

**Example:**
- 8 factors with 5-1000 values each = 28,000,000 total combinations
- Pairwise testing reduces this to ~300-500 test cases
- Still achieves high coverage of defects (studies show 70-90% of bugs involve 2 factors)

## When to Use This Skill

Use this skill when:
- You have multiple input parameters (factors) with multiple possible values (levels)
- Testing all combinations is impractical (too many test cases)
- You need systematic coverage of parameter interactions
- You're in an enterprise context where coverage must be demonstrated

## How to
```

</details>
