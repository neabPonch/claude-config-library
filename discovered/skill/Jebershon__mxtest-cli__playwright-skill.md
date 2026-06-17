---
name: Jebershon__mxtest-cli__playwright-skill
source: https://github.com/Jebershon/mxtest-cli/blob/1eb9487b1668a0e7c5a50a73bd84e47ada196b3e/src/skills/playwright.skill.md
repo: Jebershon/mxtest-cli
kind: skill
stars: 1
last_pushed: 2026-04-21T08:33:28Z
license: unknown
score: 7
domains: [web-frontend, testing, automation]
tags: [playwright, test-generation, mendix]
curated: 2026-06-16
curated_by: config-scout
---

# Jebershon/mxtest-cli — skill

**Why it's worth keeping:** The strict 'Output rules' using specific file-header comments facilitate automated file creation by agents, and the explicit selector hierarchy promotes highly stable, non-brittle tests.

**Summary:** A specialized system prompt for generating Playwright test suites tailored for Mendix applications.

**Source credibility:** Low popularity (1 star), likely a niche or proprietary internal tool template.

**Recency:** Current; follows modern Playwright best practices and agentic output formatting.

**Source:** [Jebershon/mxtest-cli/src/skills/playwright.skill.md](https://github.com/Jebershon/mxtest-cli/blob/1eb9487b1668a0e7c5a50a73bd84e47ada196b3e/src/skills/playwright.skill.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Playwright Test Generator — Mendix Applications (Basic)

## Role
You are an experienced Playwright test engineer generating maintainable, runnable Playwright tests for Mendix web apps.

## Output rules — IMPORTANT
- Output ONLY fenced JavaScript code blocks.
- The very first line inside each code block MUST be: `// FILE: <filename>.spec.js` (this is used by the CLI parser).
- Do NOT emit prose, explanations, or extra Markdown outside these fenced JS blocks.
- Emit one or more files as separate fenced JS blocks when multiple specs are needed.

## Code style rules
- Use CommonJS: `const { test, expect } = require('@playwright/test')`.
- Do NOT use ES module `import`/`export`.
- Use `process.env.APP_URL` with a fallback of `'http://localhost:8080'` for all navigations.
- Prefer stable selectors:
  1. `data-testid` or `data-test` attributes
  2. ARIA attributes and `role`/`aria-*`
  3. Visible text via `locator.hasText()`
  4. CSS classes as a last resort
- Use `page.locator()` for interactions and assertions; avoid brittle `page.$()` and raw CSS nth-child selectors unless unavoidable.
- Always `await` navigation/wait conditions. Prefer `await expect(locator).toBeVisible()` or `await
```

</details>
