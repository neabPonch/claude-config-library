---
name: joshRpowell__gamechanger
source: https://github.com/joshRpowell/gamechanger/blob/01459ef24e2d0a5fb4d97041cff246d38f93b8f7/CLAUDE.md
repo: joshRpowell/gamechanger
kind: claude-md
stars: 0
last_pushed: 2026-05-21T13:02:35Z
license: unknown
score: 8
domains: [backend-api, security, testing]
tags: [rspec, pii-protection, test-driven-development]
curated: 2026-06-14
curated_by: config-scout
---

# joshRpowell/gamechanger — claude-md

**Why it's worth keeping:** Provides high-value 'identity-as-PII' security rules that prevent leaking sensitive domain identifiers; includes a clear philosophy for bug-fix regression testing.

**Summary:** Integrates custom agentic skills (gstack) with rigorous RSpec testing protocols and strict data privacy guardrails.

**Source credibility:** Low star count but contains professional-grade, highly specific technical standards.

**Recency:** Current; aligns with modern agentic tool/skill patterns (MCP-style).

**Source:** [joshRpowell/gamechanger/CLAUDE.md](https://github.com/joshRpowell/gamechanger/blob/01459ef24e2d0a5fb4d97041cff246d38f93b8f7/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# gamechanger

## gstack

Use the `/browse` skill from gstack for all web browsing. Never use `mcp__claude-in-chrome__*` tools.

Install: `git clone https://github.com/garrytan/gstack.git ~/.claude/skills/gstack && cd ~/.claude/skills/gstack && ./setup`

Available skills: `/office-hours`, `/plan-ceo-review`, `/plan-eng-review`, `/plan-design-review`, `/design-consultation`, `/review`, `/ship`, `/browse`, `/qa`, `/qa-only`, `/design-review`, `/setup-browser-cookies`, `/retro`, `/debug`, `/document-release`

## Testing

Run tests (dev, fast):     `bundle exec rspec`
Run tests (with coverage): `COVERAGE=1 bundle exec rspec`
Test directory: `spec/`

- 100% test coverage is the goal — tests make vibe coding safe
- When writing new functions, write a corresponding test
- When fixing a bug, write a regression test (see ISSUE-001, ISSUE-002 in spec files for pattern)
- When adding error handling, write a test that triggers the error
- When adding a conditional (if/else), write tests for BOTH paths
- Never commit code that makes existing tests fail

Test conventions: RSpec with `instance_double`, `WebMock` for HTTP stubs, `Dir.mktmpdir` for temp config dirs, seeded in-memory SQLite (`':memo
```

</details>
