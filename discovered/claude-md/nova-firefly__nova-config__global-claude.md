---
name: nova-firefly__nova-config__global-claude
source: https://github.com/nova-firefly/nova-config/blob/9bca9c0966712fd6c2b485f8f7be39ea0819b580/vibe-kanban/global-claude.md
repo: nova-firefly/nova-config
kind: claude-md
stars: 1
last_pushed: 2026-06-12T22:47:31Z
license: unknown
score: 7
domains: [devops, cli-tools]
tags: [persona-automation, docker-security]
curated: 2026-06-16
curated_by: config-scout
---

# nova-firefly/nova-config — claude-md

**Why it's worth keeping:** The signal-to-skill mapping table is a highly transferable pattern for automating expert personas, while the 'Works/Blocked' list is a perfect template for teaching LLMs environmental constraints.

**Summary:** Implements an automated persona-switching system based on task signals and defines strict operational boundaries for a restricted Docker environment.

**Source credibility:** Single star; likely a personal homelab configuration.

**Recency:** Very recent (pushed 0 months ago), reflecting current Claude Code tool-use patterns.

**Source:** [nova-firefly/nova-config/vibe-kanban/global-claude.md](https://github.com/nova-firefly/nova-config/blob/9bca9c0966712fd6c2b485f8f7be39ea0819b580/vibe-kanban/global-claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Global Claude Configuration

## Auto-Skill Activation

Before responding to any technical request, automatically determine the most relevant expert
skill from `~/.claude/skills/` based on the task description and adopt that persona — no need
for the user to specify a role explicitly.

Use the following signals to pick the right skill:

| Task signals | Skill to activate |
|---|---|
| Docker Compose, container config, Traefik labels, stack management, Dockerfile | `devops-engineer` |
| Service won't start, healthcheck failing, networking issue, logs investigation | `debugging-wizard` |
| Security audit, cap_drop, secrets handling, CVE, vulnerability, hardening | `security-reviewer` + `secure-code-guardian` |
| PostgreSQL, database schema, query performance, replication | `postgres-pro` |
| React component, frontend UI, CSS, JSX/TSX | `react-expert` |
| GraphQL schema, resolver, API query | `graphql-architect` |
| Architecture trade-off, design decision, ADR | `architecture-designer` |
| TypeScript types, Node.js, npm | `typescript-pro` |
| Shell script, CLI tool, bash | `cli-developer` |
| Metrics, dashboards, alerting, logging, observability | `monitoring-expert` |
| Reliability,
```

</details>
