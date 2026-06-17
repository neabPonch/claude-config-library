---
name: abhisekjha__pith__skill
source: https://github.com/abhisekjha/pith/blob/50287ded3f72d736c52604a557573919dc32d8ec/skills/pith-debug/SKILL.md
repo: abhisekjha/pith
kind: skill
stars: 97
last_pushed: 2026-05-06T03:00:57Z
license: mit
score: 9
domains: [debugging, cli-tools, software-engineering]
tags: [structured-output, debug-protocol, low-noise]
curated: 2026-06-16
curated_by: config-scout
---

# abhisekjha/pith — skill

**Why it's worth keeping:** It mandates empirical verification via runnable commands and uses a strict schema to prevent speculative hallucinations when the cause is unknown.

**Summary:** Provides a high-density, structured format for diagnosing and fixing bugs while eliminating conversational filler.

**Source credibility:** Strong; 97 stars and recent maintenance indicate it is a vetted tool within the agentic workflow community.

**Recency:** Very current; specifically optimized for high-signal, low-noise CLI interactions required by Claude Code.

**Source:** [abhisekjha/pith/skills/pith-debug/SKILL.md](https://github.com/abhisekjha/pith/blob/50287ded3f72d736c52604a557573919dc32d8ec/skills/pith-debug/SKILL.md) · 97★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pith-debug
description: >
  One-shot structured debug format. Use when diagnosing errors, unexpected behavior, crashes, or failures.
  Format: Problem / Cause / Fix / Verify — 4 fields, no prose. Does not persist.
---

Debug format. Four fields. No prose. No preamble.

**Problem:** [what fails — one sentence, observable behavior not assumed cause]
**Cause:** [exact location — file:line if known. The specific reason it fails.]
**Fix:** [exact change — inline code, not a description of a change]
**Verify:** [runnable command or test that confirms the fix worked]

## Rules

- Each field: one line. Two lines max if critical detail requires it.
- Code inline in backticks. Block only if multi-line.
- If cause unknown: `[unknown — use verify step to investigate]` — never speculate as fact.
- Verify step must be a command or test, not "check if it works now."
- No "let me look at...", no "I see the issue is...", no trailing summary.

## Example

Bad:
> The issue seems to be related to how the token validation is being handled in the middleware layer. You might want to look at the expiry check and make sure the units are correct...

Good:
```
Problem:  JWT validation rejects valid
```

</details>
