---
name: cilangzzz__software-dev-ai-workflow__react-testing-skill
source: https://github.com/cilangzzz/software-dev-ai-workflow/blob/96c155d95314aa3d3d1666aac042aca5dfd058c1/1.0-%E8%BD%AF%E4%BB%B6%E5%BC%80%E5%8F%91%E6%B5%81%E7%A8%8B%E8%A7%92%E8%89%B2agent%E6%A8%A1%E5%9E%8B/%E6%B5%8B%E8%AF%95/skill/react-testing.skill.md
repo: cilangzzz/software-dev-ai-workflow
kind: skill
stars: 25
last_pushed: 2026-06-15T13:12:11Z
license: mit
score: 9
domains: [web-frontend, react]
tags: [react, testing, vitest, msw, accessibility]
curated: 2026-06-16
curated_by: config-scout
---

# cilangzzz/software-dev-ai-workflow — skill

**Why it's worth keeping:** Includes practical boilerplate like provider wrapping patterns, specific query priority hierarchies, and explicit instructions on mocking network layers with MSW.

**Summary:** Provides a highly opinionated and technical playbook for React testing using RTL, MSW, and Vitest.

**Source credibility:** High-quality technical content reflecting modern industry standards despite a smaller repository footprint.

**Recency:** Very current; utilizes modern tools like Vitest, userEvent, and modern MSW patterns.

**Source:** [cilangzzz/software-dev-ai-workflow/1.0-软件开发流程角色agent模型/测试/skill/react-testing.skill.md](https://github.com/cilangzzz/software-dev-ai-workflow/blob/96c155d95314aa3d3d1666aac042aca5dfd058c1/1.0-%E8%BD%AF%E4%BB%B6%E5%BC%80%E5%8F%91%E6%B5%81%E7%A8%8B%E8%A7%92%E8%89%B2agent%E6%A8%A1%E5%9E%8B/%E6%B5%8B%E8%AF%95/skill/react-testing.skill.md) · 25★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: react-testing
description: React component testing with React Testing Library, Vitest/Jest, MSW for network mocking, accessibility assertions with axe, and the decision boundary between component tests and Playwright/Cypress end-to-end runs. Use when writing or fixing tests for React components, hooks, or pages.
origin: ECC
---

# React Testing

Comprehensive React testing patterns for behavior-focused component tests, custom hook tests, accessibility assertions, and network-level mocking.

## When to Activate

- Writing tests for React components, custom hooks, or pages
- Adding test coverage to legacy untested components
- Migrating from Enzyme or class-component-era patterns to React Testing Library
- Setting up Vitest or Jest for a new React project
- Mocking HTTP requests in tests
- Asserting accessibility violations
- Deciding which tests belong in RTL vs Playwright Component Testing vs full E2E

## Core Principle

Test what the user sees and does, not implementation details.

A test should:

- Render the component with the same providers it has in production
- Interact with it via accessible queries (role, label) and `userEvent`
- Assert visible output and observab
```

</details>
