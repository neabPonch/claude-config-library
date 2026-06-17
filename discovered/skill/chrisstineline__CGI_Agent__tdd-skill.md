---
name: chrisstineline__CGI_Agent__tdd-skill
source: https://github.com/chrisstineline/CGI_Agent/blob/b582b1a4b9d45d1cc5975e64d934b818775a1c95/TDD_skill.md
repo: chrisstineline/CGI_Agent
kind: skill
stars: 0
last_pushed: 2026-05-02T18:49:22Z
license: unknown
score: 8
domains: [software-engineering, testing]
tags: [tdd, bug-fixing, quality-assurance]
curated: 2026-06-15
curated_by: config-scout
---

# chrisstineline/CGI_Agent — skill

**Why it's worth keeping:** Includes specific mental models like the 'Prove-it' pattern for bugs and clear guidance on prioritizing state-based testing over interaction-based mocks.

**Summary:** Establishes a rigorous Test-Driven Development (TDD) workflow that mandates writing failing tests before implementation or bug fixes.

**Source credibility:** Low social proof via stars, but content reflects high-level professional engineering standards.

**Recency:** Highly relevant to modern agentic development workflows.

**Source:** [chrisstineline/CGI_Agent/TDD_skill.md](https://github.com/chrisstineline/CGI_Agent/blob/b582b1a4b9d45d1cc5975e64d934b818775a1c95/TDD_skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
﻿```
---
name: test-driven-development
description: Drives development with tests. Use when implementing any logic, fixing any bug, or changing any behavior. 
Use when you need to prove that code works, when a bug report arrives, or when you're about to modify existing functionality.
---
```

# Test-Driven Development

## Overview

Write a failing test before writing the code that makes it pass. For bug fixes, reproduce the bug with a test before attempting a fix. Tests are proof — "seems right" is not done. A codebase with good tests is an AI agent's superpower; a codebase without tests is a liability.

## When to Use

- Implementing any new logic or behavior
- Fixing any bug (the Prove-It Pattern)
- Modifying existing functionality
- Adding edge case handling
- Any change that could break existing behavior

**When NOT to use:** Pure configuration changes, documentation updates, or static content changes that have no behavioral impact.

**Related:** For browser-based changes, combine TDD with runtime verification using Chrome DevTools MCP — see the Browser Testing section below.

## The TDD Cycle

```
    RED                GREEN              REFACTOR
 Write a test    Write minima
```

</details>
