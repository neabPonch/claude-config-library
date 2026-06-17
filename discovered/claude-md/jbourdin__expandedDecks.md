---
name: jbourdin__expandedDecks
source: https://github.com/jbourdin/expandedDecks/blob/2556377f7dea225dcd45cdd2650e4b234a4fd2ef/CLAUDE.md
repo: jbourdin/expandedDecks
kind: claude-md
stars: 1
last_pushed: 2026-06-15T14:49:02Z
license: apache-2.0
score: 9
domains: [backend-api, web-application, php-symfony]
tags: [symfony, coding-standards, gitflow, strict-typing]
curated: 2026-06-16
curated_by: config-scout
---

# jbourdin/expandedDecks — claude-md

**Why it's worth keeping:** The 'Use this | NOT this' table prevents tool-specific errors, and the requirement for feature traceability via '@see' tags provides excellent architectural context for an AI agent.

**Summary:** A highly disciplined instruction set that defines strict coding standards, specific CLI command wrappers, and rigid Git workflows for a Symfony/React application.

**Source credibility:** A specialized, active niche project with high-density documentation standards.

**Recency:** Very current; utilizes cutting-edge PHP 8.5/Symfony 8 syntax and modern development practices.

**Source:** [jbourdin/expandedDecks/CLAUDE.md](https://github.com/jbourdin/expandedDecks/blob/2556377f7dea225dcd45cdd2650e4b234a4fd2ef/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude AI Context

> **Audience:** Developer, AI Agent · **Scope:** Coding Standards, Workflow, Reference

## Project Overview

**Expanded Decks** is a Symfony application for managing a shared library of physical Pokemon TCG decks (Expanded format). It tracks deck ownership, event-based borrowing, and deck lists (imported via copy-paste of PTCG text format, validated against TCGdex). It includes Zebra label printing for physical deck box identification and scanning.

**Stack:** PHP 8.5 | Symfony 8.0 | React.js | MySQL 8 | Docker | PrintNode | TCGdex | ptcgo-parser

## CLI Commands: Always Use Symfony Wrapper

| Use this              | NOT this          |
|-----------------------|-------------------|
| `symfony console ...` | `bin/console ...` |
| `symfony composer ...` | `composer ...`   |
| `symfony php ...`     | `php ...`         |
| `symfony php bin/phpunit` | `bin/phpunit` |

## Naming Conventions

> Full details: [docs/standards/naming.md](docs/standards/naming.md)

| Element           | Convention        | Example                          |
|-------------------|-------------------|----------------------------------|
| Classes           | PascalCase        | `DeckLibrary`
```

</details>
