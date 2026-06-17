---
name: sjnims__plugin-dev__complete-skill
source: https://github.com/sjnims/plugin-dev/blob/7b2a8214c760d0a2f63f9dd3b6739ad5a8ff4b53/plugins/plugin-dev/skills/skill-development/examples/complete-skill.md
repo: sjnims/plugin-dev
kind: skill
stars: 15
last_pushed: 2026-06-16T04:13:56Z
license: mit
score: 8
domains: [backend-api, testing, cli-tools]
tags: [api, test-automation, rest, graphql, auth]
curated: 2026-06-16
curated_by: config-scout
---

# sjnims/plugin-dev — skill

**Why it's worth keeping:** Uses a 'progressive disclosure' pattern where core logic is separated from detailed references; includes concrete assertion templates to prevent the LLM from writing brittle tests.

**Summary:** A highly structured API testing knowledge base that provides codified patterns for authentication, assertions, and test organization.

**Source credibility:** High-quality repository structure and recent maintenance indicate an expert-level template.

**Recency:** Highly current, updated within the last month.

**Source:** [sjnims/plugin-dev/plugins/plugin-dev/skills/skill-development/examples/complete-skill.md](https://github.com/sjnims/plugin-dev/blob/7b2a8214c760d0a2f63f9dd3b6739ad5a8ff4b53/plugins/plugin-dev/skills/skill-development/examples/complete-skill.md) · 15★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Complete Skill Example

A full-featured skill demonstrating all optional components and progressive disclosure.

## Directory Structure

```text
api-testing/
├── SKILL.md
├── references/
│   ├── assertion-patterns.md
│   └── authentication-guide.md
├── examples/
│   ├── rest-api-tests.sh
│   └── graphql-tests.sh
└── scripts/
    └── generate-test.sh
```

## File Contents

### SKILL.md

````markdown
---
name: api-testing
description: This skill should be used when the user asks to "write API tests", "test REST endpoints", "test GraphQL queries", "create integration tests for APIs", "mock API responses", "test authentication flows", or needs guidance on API testing patterns, assertion strategies, or test organization.
---

# API Testing

This skill provides guidance for writing comprehensive API tests.

## Quick Start

To write an API test:

1. Identify the endpoint and expected behavior
2. Set up authentication if required
3. Make the request with appropriate headers
4. Assert response status, body, and headers
5. Clean up test data if needed

## Test Structure

Organize tests by resource and operation:

```text
tests/
├── auth/
│   ├── login.test.js
│   └── refresh-token.test.js
```

</details>
