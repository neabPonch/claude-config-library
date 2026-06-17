---
name: vidarh__writing-a-compiler-in-ruby
source: https://github.com/vidarh/writing-a-compiler-in-ruby/blob/22b8bf00fcd462597a6882ee75343b49b841a596/CLAUDE.md
repo: vidarh/writing-a-compiler-in-ruby
kind: claude-md
stars: 277
last_pushed: 2026-03-09T04:08:12Z
license: unknown
score: 9
domains: [compiler, systems-programming, ruby]
tags: [negative-constraints, architectural-integrity, testing-rules]
curated: 2026-06-15
curated_by: config-scout
---

# vidarh/writing-a-compiler-in-ruby — claude-md

**Why it's worth keeping:** Uses 'negative constraints' (e.g., NEVER/ABOMINATION) and clear bad vs. good code examples to prevent common AI shortcuts like modifying tests or hardcoding exceptions.

**Summary:** Enforces strict architectural integrity and debugging discipline by using high-intensity negative constraints.

**Source credibility:** High; part of a specialized, well-regarded technical series with significant community interest.

**Recency:** Highly relevant for modern agentic tools that interact with file systems and git history.

**Source:** [vidarh/writing-a-compiler-in-ruby/CLAUDE.md](https://github.com/vidarh/writing-a-compiler-in-ruby/blob/22b8bf00fcd462597a6882ee75343b49b841a596/CLAUDE.md) · 277★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## CRITICAL RULE: NEVER EDIT RUBYSPEC FILES

**NEVER EVER EVER EVER edit any files inside the `rubyspec/` directory.**

The RubySpec suite is a test suite that must remain unmodified:
- ❌ **NEVER** edit files in `rubyspec/` to fix failing tests
- ❌ **NEVER** add parentheses or modify test expectations
- ❌ **NEVER** work around compiler bugs by changing the specs
- ❌ **NEVER** modify rubyspec for any reason whatsoever

**If a rubyspec test fails, the ONLY acceptable solution is to fix the compiler implementation, NOT the spec.**

The specs define correct Ruby behavior. If they fail:
- ✅ Fix the implementation in `lib/core/` or compiler code
- ✅ Fix parser precedence bugs
- ✅ Fix operator implementations (like `<<`, `**`, etc.)
- ❌ **NEVER** modify the spec itself

## CRITICAL RULE: NEVER Add Special-Case Handling for Operators

**NEVER add special-case handling for individual operators in the parser or shunting yard.**

The shunting yard algorithm is designed to handle all operators generically based on:
- Precedence (priority)
- Associativity (left/right)
- Arity (nu
```

</details>
