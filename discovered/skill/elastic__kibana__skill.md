---
name: elastic__kibana__skill
source: https://github.com/elastic/kibana/blob/f3d7c438bd0794ba1e05c84321018a0c54ff9b24/src/platform/plugins/shared/workflows_management/.claude/skills/workflows-management-jest-testing/SKILL.md
repo: elastic/kibana
kind: skill
stars: 21141
last_pushed: 2026-06-15T03:34:03Z
license: other
score: 8
domains: [web-frontend, testing]
tags: [jest, react, testing-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# elastic/kibana — skill

**Why it's worth keeping:** The 'Patterns' vs 'Anti-patterns' structure is highly effective for preventing an AI from generating redundant boilerplate or incorrect provider hierarchies.

**Summary:** Provides precise instructions and patterns for using a specialized TestProvider to handle complex React context, Redux, and react-query setups in Jest tests.

**Source credibility:** Extremely high; Elastic Kibana is a major, widely-used open-source project.

**Recency:** Current; utilizes modern testing libraries and React patterns.

**Source:** [elastic/kibana/src/platform/plugins/shared/workflows_management/.claude/skills/workflows-management-jest-testing/SKILL.md](https://github.com/elastic/kibana/blob/f3d7c438bd0794ba1e05c84321018a0c54ff9b24/src/platform/plugins/shared/workflows_management/.claude/skills/workflows-management-jest-testing/SKILL.md) · 21141★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: workflows-management-jest-testing
description: Use the shared TestProvider in workflows_management Jest tests instead of hand-wiring KibanaContextProvider, QueryClientProvider, WorkflowsContextProvider, MemoryRouter, I18nProvider, and the Redux Provider. Use when writing or updating React/Jest tests under src/platform/plugins/shared/workflows_management/public/**, rendering components or hooks that touch Kibana services, the Redux store, react-query, routing, or i18n.
---

# workflows_management Jest Testing

The `workflows_management` plugin ships a single shared test provider that wires up every context a component or hook in this plugin typically needs. Use it instead of composing providers by hand.

## When to Use

Use `TestProvider` / `getTestProvider` for any Jest test under `src/platform/plugins/shared/workflows_management/public/**` that:

- renders a component or hook that reads from the Redux store,
- calls `useKibana()` / `useStartServices()` or otherwise consumes Kibana plugin services,
- uses `@kbn/react-query` (`useQuery`, `useMutation`, …),
- relies on `react-router-dom` (`useHistory`, `useParams`, links, …),
- uses `i18n` formatted messages,
- consumes `Wo
```

</details>
