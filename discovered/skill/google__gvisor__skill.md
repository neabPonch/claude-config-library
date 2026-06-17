---
name: google__gvisor__skill
source: https://github.com/google/gvisor/blob/f6e2c990bae670e263a4ac6abb27b9a91ae811ea/.claude/skills/add-syscall/SKILL.md
repo: google/gvisor
kind: skill
stars: 18536
last_pushed: 2026-06-15T20:05:05Z
license: apache-2.0
score: 9
domains: [systems-programming, kernel-dev, security]
tags: [linux, syscalls, gvisor, tdd]
curated: 2026-06-15
curated_by: config-scout
---

# google/gvisor — skill

**Why it's worth keeping:** It enforces a critical 'native-first' verification loop to ensure tests are valid on actual Linux before running in the sandbox. It also provides specific code patterns for memory management and error handling to minimize agent hallucinations.

**Summary:** A highly disciplined workflow for implementing or extending Linux syscalls within the gvisor kernel. It integrates research, implementation, and a rigorous test-driven development cycle.

**Source credibility:** High; derived from the official Google gvisor repository, a highly-starred and actively maintained project.

**Recency:** Current; utilizes modern agentic capabilities like web research and advanced tool usage for systems engineering.

**Source:** [google/gvisor/.claude/skills/add-syscall/SKILL.md](https://github.com/google/gvisor/blob/f6e2c990bae670e263a4ac6abb27b9a91ae811ea/.claude/skills/add-syscall/SKILL.md) · 18536★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
description: >
  Add or extend a Linux syscall in gvisor. Handles two cases:
  (1) Adding a brand-new syscall that currently returns ENOSYS or is missing from the table.
  (2) Adding missing flags/options to an existing partially-supported syscall (e.g., a new prctl option, ioctl command, or socket option).
  Use when asked to implement a syscall, add a flag, or improve compatibility for a specific syscall.
argument-hint: <syscall-name-or-flag>
arguments: [target]
allowed-tools:
  - Bash
  - Read
  - Edit
  - Write
  - Grep
  - Glob
  - WebSearch
  - WebFetch
  - Agent
---

# Add or extend syscall: `$target`

You are adding or extending Linux syscall support in gvisor. The target is:
**$target**

## Phase 1: Understand the current state

1.  **Check the syscall table** — search `pkg/sentry/syscalls/linux/linux64.go`
    for the syscall name. Determine:

    -   Is it registered? (has a table entry)
    -   What is its support level? (`Supported`, `PartiallySupported`,
        `ErrorWithEvent`, `Error`)
    -   What handler function is it mapped to?

2.  **Read the existing implementation** (if any) — find the handler in
    `pkg/sentry/syscalls/linux/sys_*.go`. Look for:

    -
```

</details>
