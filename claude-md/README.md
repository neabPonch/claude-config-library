# CLAUDE.md Templates

Each file in this directory is a CLAUDE.md template (or fragment) for a specific domain or stack.

## Structure

```
claude-md/
├── _base/
│   └── base.md          # Minimal base — all templates layer on top of this
├── domains/
│   ├── web-frontend/    # Browser-facing UI work
│   ├── backend-api/     # REST, GraphQL, gRPC services
│   ├── data-ml/         # Data science, ML training and inference
│   ├── devops-infra/    # IaC, CI/CD, container orchestration
│   ├── mobile/          # iOS, Android, cross-platform
│   ├── security/        # Offensive and defensive security tooling
│   ├── game-dev/        # Game engines and real-time systems
│   ├── data-engineering/# ETL, pipelines, warehouses
│   ├── cli-tools/       # Command-line utilities and scripts
│   └── agents-ai/       # LLM agents, MCP servers, orchestration
└── stacks/
    ├── react-nextjs/
    ├── python-fastapi/
    ├── go/
    ├── rust/
    ├── node-express/
    ├── django/
    ├── swift-ios/
    └── android-kotlin/
```

## File format

Every template starts with a metadata header:

```markdown
---
name: short-slug
description: one-line description of what this template covers
domain: [web-frontend, backend-api, ...]   # one or more
stack: [react-nextjs, python-fastapi, ...]  # one or more (optional)
tags: [base, fragment, complete]            # base=standalone, fragment=layer-on-top, complete=full template
---
```

## Layering model

The advisor composes configs by layering:

1. `_base/base.md` — always included
2. Domain template(s) — layered on top
3. Stack template(s) — layered on top

Sections with the same heading are merged (later layers win for conflicts).
