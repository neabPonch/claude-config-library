---
name: LambdaTest__agent-skills__skill
source: https://github.com/LambdaTest/agent-skills/blob/86f9302541e792923b570f4db49dc4e93a959a24/nightwatchjs-skill/SKILL.md
repo: LambdaTest/agent-skills
kind: skill
stars: 312
last_pushed: 2026-06-08T11:45:52Z
license: mit
score: 8
domains: [e2e-testing, web-automation]
tags: [nightwatchjs, javascript, selenium, page-objects]
curated: 2026-06-16
curated_by: config-scout
---

# LambdaTest/agent-skills — skill

**Why it's worth keeping:** It defines clear execution paths (local vs cloud) and provides structured code templates for page objects and assertions to ensure the agent writes consistent, professional-grade automation.

**Summary:** Provides a comprehensive template for generating NightwatchJS E2E tests including environment configurations and Page Object patterns.

**Source credibility:** High; authored by TestMu AI/LambdaTest, experts in automated testing infrastructure.

**Recency:** Current; reflects modern JavaScript/TypeScript E2E automation standards.

**Source:** [LambdaTest/agent-skills/nightwatchjs-skill/SKILL.md](https://github.com/LambdaTest/agent-skills/blob/86f9302541e792923b570f4db49dc4e93a959a24/nightwatchjs-skill/SKILL.md) · 312★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: nightwatchjs-skill
description: >
  Generates NightwatchJS E2E tests in JavaScript. Integrated test runner with
  Selenium WebDriver, built-in assertions, and page objects. Use when user
  mentions "Nightwatch", "NightwatchJS", "nightwatch.conf.js". Triggers on:
  "Nightwatch", "NightwatchJS", "nightwatch test".
languages:
  - JavaScript
  - TypeScript
category: e2e-testing
license: MIT
metadata:
  author: TestMu AI
  version: "1.0"
---

# NightwatchJS Automation Skill

## Step 1 — Execution Target

```
├─ "cloud", "TestMu", "LambdaTest" → Cloud: nightwatch.conf.js with LT env
├─ "local" → Local: ChromeDriver/GeckoDriver
└─ Default → Local, mention cloud option
```

## Core Patterns

### Basic Test

```javascript
module.exports = {
  'Login with valid credentials': function(browser) {
    browser
      .url('http://localhost:3000/login')
      .waitForElementVisible('#email', 5000)
      .setValue('#email', 'user@test.com')
      .setValue('#password', 'password123')
      .click('button[type="submit"]')
      .waitForElementVisible('.dashboard', 10000)
      .assert.containsText('.welcome', 'Welcome')
      .assert.urlContains('/dashboard')
      .end();
  },

  'Login w
```

</details>
