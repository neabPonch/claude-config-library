---
name: codexstar69__bug-hunter
source: https://github.com/codexstar69/bug-hunter/blob/8dedbbb10e93a3465e4549778587a4c40d0e673f/SKILL.md
repo: codexstar69/bug-hunter
kind: skill
stars: 423
last_pushed: 2026-05-01T12:18:26Z
license: mit
score: 9
domains: [security, agents-ai, cli-tools]
tags: [adversarial-verification, bug-hunting, workflow-automation]
curated: 2026-06-16
curated_by: config-scout
---

# codexstar69/bug-hunter — skill

**Why it's worth keeping:** The implementation of an adversarial 'Skeptic' stage to challenge findings before fixing, and the highly structured logic for handling complex state transitions like dry-runs, plan-only modes, and threat modeling.

**Summary:** An adversarial bug-hunting pipeline that uses a sequential multi-agent workflow (Recon, Hunter, Skeptic, Referee) to find, verify, and auto-fix bugs. It features sophisticated command-line argument parsing for granular control over security reviews, PR assessments, and execution modes.

**Source credibility:** High; 423 stars indicates significant community validation and utility.

**Recency:** Very current; uses modern developer workflows including PR/branch diffing and security auditing.

**Source:** [codexstar69/bug-hunter/SKILL.md](https://github.com/codexstar69/bug-hunter/blob/8dedbbb10e93a3465e4549778587a4c40d0e673f/SKILL.md) · 423★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: bug-hunter
description: "Adversarial bug hunting with a sequential-first pipeline (Recon, Hunter, Skeptic, Referee) that can optionally use safe read-only parallel triage. Finds, verifies, and auto-fixes real bugs by default (with --scan-only opt-out) using checkpointed verification and resume state for large codebases. Use this skill whenever the user wants bug finding, security audits, regression checks, or code review focused on runtime behavior."
---

# Bug Hunt - Adversarial Bug Finding

Run a sequential-first adversarial bug hunt on your codebase. Use parallelism only for read-only triage and independent verification tasks.

## Table of Contents
- [Usage](#usage)
- [Target](#target)
- [Context Budget](#context-budget)
- [Execution Steps](#execution-steps)
- [Step 7: Present the Final Report](#step-7-present-the-final-report)
- [Self-Test Mode](#self-test-mode)
- [Error handling](#error-handling)

**Phase 1 — Find & Verify:**
```
Recon (map) --> Hunter (deep scan) --> Skeptic (challenge) --> Referee (final verdict)
                    ^                 (optional read-only dual-lens triage can run here)
                    |
             state + chunk checkpoints
```
```

</details>
