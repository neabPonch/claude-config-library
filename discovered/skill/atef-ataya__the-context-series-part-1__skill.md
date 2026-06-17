---
name: atef-ataya__the-context-series-part-1__skill
source: https://github.com/atef-ataya/the-context-series-part-1/blob/0a3254470b56949c753c3f723904c735f421cb95/claude/Skill.md
repo: atef-ataya/the-context-series-part-1
kind: skill
stars: 0
last_pushed: 2026-01-18T19:49:00Z
license: unknown
score: 7
domains: [web-frontend, typescript, nextjs]
tags: [code-review, react, typescript]
curated: 2026-06-17
curated_by: config-scout
---

# atef-ataya/the-context-series-part-1 — skill

**Why it's worth keeping:** It utilizes specific 'Component Conventions' and a rigid 'Output Format' to ensure the agent enforces stylistic consistency rather than just checking logic.

**Summary:** Provides a highly structured review workflow specifically optimized for modern Next.js and TypeScript stacks.

**Source credibility:** Low; single-author repository with zero stars and limited social proof.

**Recency:** Very recent, targeting bleeding-edge versions like React 19 and Tailwind CSS 4.

**Source:** [atef-ataya/the-context-series-part-1/claude/Skill.md](https://github.com/atef-ataya/the-context-series-part-1/blob/0a3254470b56949c753c3f723904c735f421cb95/claude/Skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: code-review
description: Code review for Next.js and TypeScript projects. Use when asked to "review this code", "check this PR", "review my changes", "look at this component", or any code review request. Applies team standards for TypeScript types, React component patterns, error handling, accessibility, and performance.
metadata:
  author: atef-ataya
  version: '1.0.0'
---

# Code Review

## Review Process

1. **Understand Intent** — What is this code trying to accomplish?
2. **Check Standards** — TypeScript types, component patterns, error handling
3. **Review Logic** — Bugs, edge cases, correctness
4. **Security Scan** — Common vulnerabilities (XSS, injection, exposed secrets)
5. **Synthesize Feedback** — Actionable recommendations

## Output Format

Always structure reviews as follows:

### Summary

One paragraph: What does this code do? Is it ready to merge?

### Critical Issues (Must Fix)

- Security vulnerabilities
- Logic errors / bugs
- Breaking changes

### Improvements (Should Fix)

- Missing TypeScript types
- Component structure issues
- Missing error handling

### Suggestions (Nice to Have)

- Performance optimizations
- Refactoring opportunities
- Better na
```

</details>
