---
name: Mindrally__skills__skill
source: https://github.com/Mindrally/skills/blob/05a71308897983093248d719a2ffa1bca61d0768/cypress/SKILL.md
repo: Mindrally/skills
kind: skill
stars: 141
last_pushed: 2026-06-09T21:37:11Z
license: apache-2.0
score: 8
domains: [web-frontend, testing]
tags: [cypress, e2e, javascript]
curated: 2026-06-15
curated_by: config-scout
---

# Mindrally/skills — skill

**Why it's worth keeping:** Provides specific code templates for modern patterns like `cy.session` and `cy.intercept`, while explicitly banning common anti-patterns like arbitrary timeouts.

**Summary:** Establishes strict guidelines for Cypress E2E testing, prioritizing selector stability and network intercepting over brittle CSS paths.

**Source credibility:** The source is an active, well-starred repository of specialized rules.

**Recency:** Current; utilizes modern Cypress features essential for reliable testing today.

**Source:** [Mindrally/skills/cypress/SKILL.md](https://github.com/Mindrally/skills/blob/05a71308897983093248d719a2ffa1bca61d0768/cypress/SKILL.md) · 141★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cypress
description: Cypress end-to-end testing best practices for web applications, covering test structure, commands, and reliability patterns.
---

# Cypress Testing Best Practices

You are an expert in Cypress end-to-end testing.

## Core Principles

### Test Structure
- Use descriptive test names that clearly explain expected behavior
- Organize tests by feature or user flow
- Keep tests focused on critical user paths
- Follow the Given-When-Then pattern for clarity

### Selecting Elements
- Prefer `data-testid` or `data-cy` attributes for test selectors
- Use `cy.contains()` for text-based selection when appropriate
- Avoid brittle selectors like CSS classes or tag hierarchies

```javascript
// Recommended
cy.get('[data-testid="submit-button"]').click();
cy.contains('Submit').click();

// Avoid
cy.get('.btn-primary').click();
```

### Commands and Assertions
- Chain commands fluently for readability
- Use built-in retry-ability; avoid explicit waits
- Prefer `.should()` assertions over `.then()` for automatic retries
- Use `.within()` to scope commands to a specific element

### Custom Commands
- Create custom commands for repeated actions
- Place custom commands in
```

</details>
