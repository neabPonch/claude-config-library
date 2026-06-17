---
name: talk2MeGooseman__stream_closed_captioner_phoenix__skill
source: https://github.com/talk2MeGooseman/stream_closed_captioner_phoenix/blob/30eed5c7a0e44867a01a4e4721e2ad3cc4569cd7/.github/skills/elixir-phoenix-best-practices/SKILL.md
repo: talk2MeGooseman/stream_closed_captioner_phoenix
kind: skill
stars: 24
last_pushed: 2026-06-13T20:03:04Z
license: gpl-3.0
score: 8
domains: [backend, web-development, elixir]
tags: [elixir, phoenix, architecture, code-review]
curated: 2026-06-15
curated_by: config-scout
---

# talk2MeGooseman/stream_closed_captioner_phoenix — skill

**Why it's worth keeping:** It enforces high-level pattern matching (tagged tuples) and specific data integrity practices like Ecto.Multi usage and N+1 prevention.

**Summary:** This skill provides a structured audit workflow for Elixir/Phoenix applications, focusing on architectural layer separation and reliability.

**Source credibility:** Derived from a real-world Phoenix application, though it is a niche repository with modest star count.

**Recency:** Highly current; follows modern Elixir/Phoenix architectural standards.

**Source:** [talk2MeGooseman/stream_closed_captioner_phoenix/.github/skills/elixir-phoenix-best-practices/SKILL.md](https://github.com/talk2MeGooseman/stream_closed_captioner_phoenix/blob/30eed5c7a0e44867a01a4e4721e2ad3cc4569cd7/.github/skills/elixir-phoenix-best-practices/SKILL.md) · 24★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: elixir-phoenix-best-practices
description: "Use when: enforcing Elixir and Phoenix best practices, reviewing contexts/controllers/liveviews, improving changesets/queries, and preparing production-ready Elixir code"
license: MIT
---

# Elixir Phoenix Best Practices

## Overview

Apply a repeatable workflow to audit and improve Elixir/Phoenix code quality without changing intended behavior.

## Use This Skill For

- Elixir/Phoenix code reviews
- Context/controller boundary checks
- Query and changeset quality checks
- Error handling consistency improvements
- Maintainability hardening before merge

## Workflow

1. Identify the touched modules and classify each as web layer, domain/context layer, data layer, or integration layer.
2. Verify architectural boundaries:
- Web layer delegates business decisions to context/service modules.
- Context APIs remain stable and explicit.
3. Verify correctness and reliability:
- Fallible flows return tagged tuples.
- Pattern matching and `with` are used for clarity in multi-step logic.
- External input is validated through changesets or dedicated validators.
4. Verify data access:
- Queries avoid N+1 patterns.
- Transactional writes use `
```

</details>
