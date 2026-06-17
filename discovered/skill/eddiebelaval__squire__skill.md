---
name: eddiebelaval__squire__skill
source: https://github.com/eddiebelaval/squire/blob/8c974b2c36fd9147fbea5a9ec42158a1103a674e/skills/heal/skill.md
repo: eddiebelaval/squire
kind: skill
stars: 17
last_pushed: 2026-06-06T11:02:18Z
license: mit
score: 9
domains: [testing, cli-tools, developer-experience]
tags: [tdd, autonomous, debugging, test-fixing]
curated: 2026-06-16
curated_by: config-scout
---

# eddiebelaval/squire — skill

**Why it's worth keeping:** Implements critical guardrails like dependency-based prioritization (types first) and a '3-strike' escalation rule to prevent infinite loops. It also uses a structured logging pattern with FIXES.md for auditability.

**Summary:** An autonomous red-to-green loop that runs tests, fixes source code failures, and verifies the environment via type-checking.

**Source credibility:** High; the source repository claims extensive real-world session data and deep tool integration.

**Recency:** Very current, targeting modern TypeScript and Playwright workflows.

**Source:** [eddiebelaval/squire/skills/heal/skill.md](https://github.com/eddiebelaval/squire/blob/8c974b2c36fd9147fbea5a9ec42158a1103a674e/skills/heal/skill.md) · 17★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: Heal
slug: heal
description: Autonomous test-fix loop — run tests, fix failures, repeat until green
category: testing
complexity: complex
version: "1.0.0"
author: "id8Labs"
triggers:
  - "heal"
  - "fix tests"
  - "fix all tests"
  - "make tests pass"
  - "red to green"
tags:
  - testing
  - autonomous
  - fix
  - tdd
---

# Heal — Autonomous Test Fix Loop

Run the full test suite, fix every failure at the source, and repeat until green. No guidance needed — fully autonomous red-green loop.

## Core Workflows

### Workflow 1: Full Heal (Default)
1. Detect environment and available test commands
2. Run full test suite
3. Parse failures
4. Fix each failure at the source
5. Re-run tests
6. Repeat until green or max iterations reached
7. Commit fixes (unless --no-commit)

## Usage

```
/heal                    # Fix all failing tests in current project
/heal --unit-only        # Only run unit tests (skip Playwright)
/heal --no-commit        # Fix everything but don't commit at the end
/heal --dry-run          # Show what's failing without fixing anything
```

## Instructions

When invoked:

### Step 0: Detect Environment

1. Identify the project from the current directory (ch
```

</details>
