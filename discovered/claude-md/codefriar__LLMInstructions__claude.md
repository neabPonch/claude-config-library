---
name: codefriar__LLMInstructions__claude
source: https://github.com/codefriar/LLMInstructions/blob/ee3e9a8b558b3fff54a97a6ff86644f5224ce35e/Salesforce/CLAUDE.md
repo: codefriar/LLMInstructions
kind: claude-md
stars: 8
last_pushed: 2025-08-22T19:49:20Z
license: mit
score: 9
domains: [salesforce, backend-api, cli-tools]
tags: [apex, sfdx, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# codefriar/LLMInstructions — claude-md

**Why it's worth keeping:** It provides highly actionable `sf` CLI command templates, strict folder organization rules, and clear implementation patterns for Repository and Service layers.

**Summary:** A comprehensive guide for Salesforce Apex development that covers toolsets, architecture, and testing requirements.

**Source credibility:** Moderate; based on a community-curated repository of LLM instructions.

**Recency:** Current, referencing modern Salesforce DX (sf) CLI usage and high API versions.

**Source:** [codefriar/LLMInstructions/Salesforce/CLAUDE.md](https://github.com/codefriar/LLMInstructions/blob/ee3e9a8b558b3fff54a97a6ff86644f5224ce35e/Salesforce/CLAUDE.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Salesforce Apex Development Guidelines for Claude

The following guidelines should be followed when helping with Salesforce Apex development:

## Language Limitations

- Apex has very limited reflection capabilities.
- When the need arises to test a private method, add the `@TestVisible` annotation to the line above the method to be tested's definition. This will effectively make the method `public` for the duration of a unit test.
- Use private constructors with the `@TestVisible` annotation to provide test-only dependency injection enabled constructors.

## Platform oddities

- Salesforce projects, while developed locally, must be deployed to an org for testing.
- Salesforce requires that All Apex code have an Aggregate code coverage of >= 75%. Writing or refactoring an Apex class therefore means also writing or refactoring the tests.
- More importantly, regardless of code coverage percentage, I require that _all logic branches_ in the code have coverage.
- Test classes should follow the naming convetion ClassNameTests. Example: IdServiceTests, or AccountServiceTests
- Salesforce provides a bash cli tool for interacting with project metadata called `sf`. you may safely assume `
```

</details>
