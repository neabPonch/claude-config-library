# Contributing

## Adding a CLAUDE.md template

1. Find the right folder under `claude-md/domains/` or `claude-md/stacks/`
2. Create `[descriptive-name].md` with the required metadata header (see [`claude-md/README.md`](claude-md/README.md))
3. Add an entry to `catalog.json` under `claude-md.domains` or `claude-md.stacks`
4. Open a PR — title format: `claude-md: add [domain/stack] template`

## Adding a skill

1. Find the right folder under `skills/domains/` or `skills/stacks/`
2. Create `[skill-name].md` with the required metadata header (see [`skills/README.md`](skills/README.md))
3. Add an entry to `catalog.json`
4. Open a PR — title format: `skill: add [name]`

## Adding a workflow

1. Add to `workflows/practices/`, `workflows/patterns/`, or `workflows/integrations/`
2. Follow the format in [`workflows/README.md`](workflows/README.md)
3. Add an entry to `catalog.json`
4. Open a PR — title format: `workflow: add [name]`

## Quality bar

- Templates should be **battle-tested**, not speculative — ideally sourced from real projects
- Cite the source or research behind non-obvious recommendations
- Avoid generic filler; every line should earn its place
- Keep metadata headers accurate — the advisor depends on them

## Metadata header requirements

Every template file must begin with:

```markdown
---
name: short-kebab-slug
description: one-line description (used by the advisor for matching)
domain: [list of applicable domains]
stack: [list of applicable stacks, if stack-specific]
tags: [relevant tags]
---
```
