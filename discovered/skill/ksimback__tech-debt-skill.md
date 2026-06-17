---
name: ksimback__tech-debt-skill
source: https://github.com/ksimback/tech-debt-skill/blob/5a15c1ca4a929b2759461c218478de391a8bda0f/SKILL.md
repo: ksimback/tech-debt-skill
kind: skill
stars: 514
last_pushed: 2026-04-25T22:17:13Z
license: unknown
score: 9
domains: [developer-tools, software-engineering]
tags: [audit, tech-debt, codebase-analysis, refactoring]
curated: 2026-06-14
curated_by: config-scout
---

# ksimback/tech-debt-skill — skill

**Why it's worth keeping:** The 'Orientation' phase prevents superficial pattern-matching by analyzing file churn and actual architecture first; the mandatory 'looks bad but is fine' section effectively eliminates false positives common in LLM audits.

**Summary:** A rigorous, multi-phase technical debt audit protocol that prioritizes understanding system context through git churn and architecture mapping before issuing critiques. It produces a high-density, cited report designed for actionable engineering decisions.

**Source credibility:** High; 500+ stars and recent updates suggest a widely adopted, reliable tool.

**Recency:** 

**Source:** [ksimback/tech-debt-skill/SKILL.md](https://github.com/ksimback/tech-debt-skill/blob/5a15c1ca4a929b2759461c218478de391a8bda0f/SKILL.md) · 514★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: tech-debt-audit
description: Thorough, user-invoked tech debt and architecture audit of the current codebase. Produces TECH_DEBT_AUDIT.md with file-cited findings, severity, effort estimates, and a required "looks bad but is actually fine" section. Use when the user asks for a debt audit, codebase health check, architecture review, or code quality assessment of an entire repo. Does not auto-invoke.
disable-model-invocation: true
---

# Tech Debt Audit

A Claude Code skill that conducts a deliberate, opinionated audit of an entire codebase and produces `TECH_DEBT_AUDIT.md` with cited findings.

When invoked via `/tech-debt-audit`, follow the protocol below. Everything from here through the `---` divider is the protocol Claude executes. The section after the divider is documentation for humans installing or maintaining this skill.

---

## Operating principles

Find what's actually wrong. Not diplomatic. Not surface-only. Don't pattern-match to generic best practices without grounding in this specific repo. No sycophancy. No "overall the codebase is well-structured" filler.

Cite `file:line` for every concrete finding. Vague claims like "the code generally..." don't count.
```

</details>
