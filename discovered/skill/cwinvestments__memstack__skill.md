---
name: cwinvestments__memstack__skill
source: https://github.com/cwinvestments/memstack/blob/a01b858371b7796668942b1f3c8dce006ecb3196/skills/verify/SKILL.md
repo: cwinvestments/memstack
kind: skill
stars: 384
last_pushed: 2026-05-31T02:33:13Z
license: mit
score: 9
domains: [software-development, quality-assurance]
tags: [verification, testing, sdlc, pre-commit]
curated: 2026-06-15
curated_by: config-scout
---

# cwinvestments/memstack — skill

**Why it's worth keeping:** The 'Anti-Rationalization' section is a high-tier technique to prevent LLM shortcuts, while the structured report ensures consistent output quality.

**Summary:** An end-to-end verification skill that combines automated build/test execution with manual requirement validation and common issue scanning.

**Source credibility:** High; 384 stars and active development indicate a respected framework.

**Recency:** Highly current, utilizing modern CLI tool detection and Git-based context analysis.

**Source:** [cwinvestments/memstack/skills/verify/SKILL.md](https://github.com/cwinvestments/memstack/blob/a01b858371b7796668942b1f3c8dce006ecb3196/skills/verify/SKILL.md) · 384★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: verify
description: "Use when the user says 'verify', 'check this work', 'does it pass', or before committing completed work."
version: 1.0.0
---


# ✅ Verify — Checking Work...
*Review completed work against requirements before committing.*

## Activation

When this skill activates, output:

`✅ Verify — Checking work against requirements...`

Then execute the protocol below.

## Context Guard

| Context | Status | Priority |
|---------|--------|----------|
| **User says "verify", "check this work", "does it pass"** | ACTIVE — run verification | P1 |
| **User says "is this done", "ready to commit"** | ACTIVE — run verification | P1 |
| **User is mid-task, still actively coding** | DORMANT — let them finish first | — |
| **User asks to commit or push** | DORMANT — Seal hook handles pre-push checks | — |
| **User asks to review someone else's code** | DORMANT — not a code review tool | — |

## Anti-Rationalization

If you're thinking any of these, STOP — you're about to skip the protocol:

| You're thinking... | Reality |
|---|---|
| "I already tested this manually" | Ad-hoc testing leaves no record. Run the automated checks. |
| "This change is too small to verify" | Small
```

</details>
