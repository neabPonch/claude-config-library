---
name: streamband__hydra-srt__skill
source: https://github.com/streamband/hydra-srt/blob/3685c5687bc5a81a29e9ce8bc299dc9a2e7d5ed0/.agents/skills/elixir/SKILL.md
repo: streamband/hydra-srt
kind: skill
stars: 73
last_pushed: 2026-06-13T10:01:03Z
license: apache-2.0
score: 8
domains: [backend, web-development]
tags: [elixir, phoenix, ecto, otp]
curated: 2026-06-16
curated_by: config-scout
---

# streamband/hydra-srt — skill

**Why it's worth keeping:** It specifies precise syntax preferences (like map access patterns), provides exact CLI commands for the toolchain, and mandates strict architectural rules like keeping logic in contexts rather than controllers.

**Summary:** A highly opinionated guide for Elixir/Phoenix development that enforces architectural boundaries and specific coding styles.

**Source credibility:** The source is an active open-source project related to SRT streaming gateway development with respectable star counts.

**Recency:** Highly current; reflects modern Elixir/OTP best practices.

**Source:** [streamband/hydra-srt/.agents/skills/elixir/SKILL.md](https://github.com/streamband/hydra-srt/blob/3685c5687bc5a81a29e9ce8bc299dc9a2e7d5ed0/.agents/skills/elixir/SKILL.md) · 73★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: elixir
description: Use this skill for Elixir/Phoenix development in this repo: implementing features, refactors, debugging, tests, Ecto changes, and production-safe fixes.
---

# Elixir Skill

## When to use
Use for any task touching Elixir, Phoenix, Ecto, Mix, OTP, or ExUnit.

## Workflow
1. Read context first: routes, schema, context modules, and related tests.
2. Keep business logic in contexts, not in controllers/channels/live views.
3. Prefer small pure functions and explicit pattern matching.
4. Prefer bracket access (`map[:key]`) for map reads in app code. Do not use `Map.get/2`. Use `Map.get/3` only when an explicit default value is required.
5. Add `@spec` for every function (`def`/`defp`).
6. If a `@spec` becomes hard to read, introduce named custom types (`@type`, `@opaque`) and reuse them in specs.
7. Add or update tests with each behavior change.
8. Run targeted tests first, then broader suite if needed.

## Repo commands
- Format: `mix format`
- Compile with warnings: `mix compile --warnings-as-errors`
- Run tests: `mix test`
- Run specific test file: `mix test path/to/test_file.exs`
- Run one test line: `mix test path/to/test_file.exs:123`

## Ecto and DB
```

</details>
