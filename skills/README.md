# Skills

Skill files are reusable Claude Code `/skill` definitions. Each file defines a skill that Claude Code can invoke with a slash command.

## Structure

```
skills/
├── domains/
│   ├── web-frontend/
│   ├── backend-api/
│   ├── data-ml/
│   ├── devops-infra/
│   ├── mobile/
│   ├── security/
│   ├── game-dev/
│   ├── data-engineering/
│   ├── cli-tools/
│   └── agents-ai/
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

```markdown
---
name: skill-slug
command: /command-name
description: one-line description shown in /help
domain: [web-frontend, ...]
stack: [react-nextjs, ...]   # optional
tags: [debug, review, generate, refactor, test, deploy, document]
---

# Skill: command-name

[Full skill prompt — instructions Claude follows when this skill is invoked]

## Arguments

- `$1` — [description of first argument, if any]

## What this skill does

[Bullet list of what Claude will do when invoked]

## Example usage

/command-name [example args]
```

## Skill categories (tags)

| Tag | Examples |
|-----|---------|
| `debug` | trace an error, diagnose a flaky test |
| `review` | code review, security audit, perf audit |
| `generate` | scaffold a component, create a migration |
| `refactor` | extract module, rename consistently |
| `test` | generate test cases, increase coverage |
| `deploy` | release checklist, rollback guide |
| `document` | generate API docs, write a changelog |
| `research` | summarize an RFC, compare libraries |
