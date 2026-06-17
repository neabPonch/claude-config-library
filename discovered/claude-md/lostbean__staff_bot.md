---
name: lostbean__staff_bot
source: https://github.com/lostbean/staff_bot/blob/968ddc8a1e119addf1777f4fa0f49ee872b7f933/CLAUDE.md
repo: lostbean/staff_bot
kind: claude-md
stars: 0
last_pushed: 2025-06-14T13:45:01Z
license: unknown
score: 8
domains: [backend-api, ai-agents]
tags: [elixir, phoenix, reactor-pattern, testing-mimic]
curated: 2026-06-16
curated_by: config-scout
---

# lostbean/staff_bot — claude-md

**Why it's worth keeping:** Includes a 'Correct vs NOT' syntax guide for testing and a concrete code template for error handling that prevents architectural regressions.

**Summary:** Defines specific architectural patterns (Reactor) and provides explicit mocking/testing instructions for the Mimic library.

**Source credibility:** Low star count, but technical density suggests it is a high-quality internal documentation file rather than boilerplate.

**Recency:** 12 months old; the Elixir patterns and implementation details remain highly relevant for Claude Code.

**Source:** [lostbean/staff_bot/CLAUDE.md](https://github.com/lostbean/staff_bot/blob/968ddc8a1e119addf1777f4fa0f49ee872b7f933/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Instructions for StaffBot Development

## Project Overview
StaffBot is an Elixir Phoenix application that provides AI-powered code review for GitHub pull requests. The application uses the Reactor pattern for composable, reusable workflow steps and Mimic for testing.

## Key Architecture Patterns

### Reactor Pattern Implementation
- **Purpose**: Create composable, reusable workflow steps for GitHub AI review processes
- **Location**: `lib/github/steps/` and `lib/github/*_reactor.ex`
- **Step Modules**: Each step implements `use Reactor.Step` with `run/3` function signature
- **Static Values**: Use `argument(:key, value("static_string"))` for static arguments in DSL
- **Dependencies**: Use `argument(:key, result(:previous_step))` and `argument(:key, input(:input_name))`

### Log stacktrace
Make sure to log stacktraces from unexpected errors by adding `rescue` at the of the implemented Step callbacks. For example:
```elixir
  @impl Reactor.Step
  def run(%{rules: rules, code: code}, _context, _step) do
      # Some logic here
  rescue
    e ->
      Exception.format(:error, e, __STACKTRACE__) |> Logger.warning()
      {:error, e}
  end
```

### Current Reactor Workflows
2.
```

</details>
