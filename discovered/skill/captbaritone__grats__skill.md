---
name: captbaritone__grats__skill
source: https://github.com/captbaritone/grats/blob/f650d2e47feb2cccb12bda74c79e278d738daaf2/skills/grats/SKILL.md
repo: captbaritone/grats
kind: skill
stars: 357
last_pushed: 2026-05-31T17:43:09Z
license: mit
score: 9
domains: [backend-api, typescript, graphql]
tags: [graphql, type-safety, schema-generation]
curated: 2026-06-15
curated_by: config-scout
---

# captbaritone/grats — skill

**Why it's worth keeping:** Uses a meta-technique of pointing the agent toward structured documentation within `node_modules` to prevent prompt bloat. It also preemptively addresses non-obvious behaviors like nullability and root type auto-creation.

**Summary:** Provides deep context for the Grats GraphQL library, including docblock tag mappings, configuration rules, and CLI workflows.

**Source credibility:** High; actively maintained with significant community traction for a niche tool.

**Recency:** Current; utilizes modern local documentation discovery patterns.

**Source:** [captbaritone/grats/skills/grats/SKILL.md](https://github.com/captbaritone/grats/blob/f650d2e47feb2cccb12bda74c79e278d738daaf2/skills/grats/SKILL.md) · 357★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: grats
description: Build GraphQL servers by annotating TypeScript code with docblock tags like @gqlType and @gqlField. Use when writing, reviewing, or refactoring GraphQL resolvers in a project that uses Grats, or when the user mentions Grats, @gqlType, @gqlField, or similar docblock tags.
license: MIT
metadata:
  author: grats
  version: "1.0.0"
---

# Grats

Grats extracts a GraphQL schema from TypeScript code. Instead of writing a separate schema file, you annotate your TypeScript types and functions with docblock tags like `/** @gqlType */` and `/** @gqlField */`. Grats then generates an executable GraphQL schema and a `.graphql` file as a build step.

## Documentation

Grats ships comprehensive documentation in its npm package at `node_modules/grats/llm-docs/`. Read these files for detailed reference:

- **Getting started**: `node_modules/grats/llm-docs/getting-started/quick-start.md`
- **All docblock tags**: `node_modules/grats/llm-docs/docblock-tags.md`
- **Resolver patterns**: `node_modules/grats/llm-docs/resolvers.md`
- **Configuration**: `node_modules/grats/llm-docs/getting-started/configuration.md`
- **CLI usage**: `node_modules/grats/llm-docs/getting-started/c
```

</details>
