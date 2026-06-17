---
name: commercetools__ui-kit
source: https://github.com/commercetools/ui-kit/blob/92ac7decd9ec3a538235a73141215c7f5046ebdf/CLAUDE.md
repo: commercetools/ui-kit
kind: claude-md
stars: 153
last_pushed: 2026-06-12T18:28:51Z
license: mit
score: 9
domains: [web-frontend, agents-ai, devops]
tags: [mcp, skills-system, agentic-workflow, automation]
curated: 2026-06-15
curated_by: config-scout
---

# commercetools/ui-kit — claude-md

**Why it's worth keeping:** It demonstrates the high-level pattern of offloading complex domain tasks (like Renovate migrations or Jira management) into discrete 'Skills'. The integration of MCP servers for documentation and visual verification is a top-tier professional technique.

**Summary:** This config establishes an agentic ecosystem by integrating MCP servers, post-tool hooks for auto-formatting, and a managed 'Skills' system. It serves as a registry that tells Claude how to use specialized enterprise tools rather than just project rules.

**Source credibility:** High; commercetools is an enterprise-grade source with active maintenance and high star count.

**Recency:** Very current, utilizing modern agentic patterns like MCP and custom skill orchestration.

**Source:** [commercetools/ui-kit/CLAUDE.md](https://github.com/commercetools/ui-kit/blob/92ac7decd9ec3a538235a73141215c7f5046ebdf/CLAUDE.md) · 153★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Configuration

Read `AGENTS.md` for full project context — it is the primary reference for this
repository's architecture, commands, constraints, and conventions.

## MCP Servers

See `.mcp.json` for configured servers:

- **commercetools-docs** — commercetools API docs, GraphQL schemas, OpenAPI
  specs
- **context7** — third-party library documentation
- **playwright** — visual UI verification
- **sequential-thinking** — structured multi-step reasoning

## Hooks

See `.claude/settings.json` for configured hooks:

- PostToolUse (Edit/MultiEdit/Write): auto-format with Prettier

## Skills

Skills live in `.agents/skills/` and are symlinked into `.claude/skills/`.
Update with `npx skills update` — check `git diff` afterward for lost repo-specific content.

Shared skills installed via `skills add commercetools/agent-skills/skills/<name>`:

- `/repo-healthcheck-node` — verify repo setup
- `/remember` — persistent memory across sessions
- `/repo-maintenance-node` — formatting, dead code, dependency validation
- `/jira-create-epic-from-plan` — create Jira epic from markdown plan
- `/jira-implement-task` — implement a Jira ticket end-to-end
- `/renovate-review` — review Reno
```

</details>
