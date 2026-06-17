---
name: confluentinc__vscode
source: https://github.com/confluentinc/vscode/blob/84814fce3dc6ca46ca0d1757e5d420cf172d7c02/CLAUDE.md
repo: confluentinc/vscode
kind: claude-md
stars: 34
last_pushed: 2026-06-15T06:02:28Z
license: apache-2.0
score: 9
domains: [vscode-extension, typescript]
tags: [disposable-pattern, architecture-rules, resource-management]
curated: 2026-06-15
curated_by: config-scout
---

# confluentinc/vscode — claude-md

**Why it's worth keeping:** The inclusion of a 'Mandatory' code example for the Disposable pattern is highly effective at preventing subtle bugs. It also mandates specific telemetry/error utilities rather than generic logging, ensuring consistency across the codebase.

**Summary:** Provides strict architectural guardrails and specific implementation patterns for a VS Code extension. It focuses heavily on resource management via the Disposable pattern to prevent memory leaks.

**Source credibility:** High-quality professional engineering standard from Confluent; reflects a mature development workflow.

**Recency:** Highly current; explicitly optimized for Claude Code and modern TypeScript workflows.

**Source:** [confluentinc/vscode/CLAUDE.md](https://github.com/confluentinc/vscode/blob/84814fce3dc6ca46ca0d1757e5d420cf172d7c02/CLAUDE.md) · 34★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this
repository.

## Project Overview

**Confluent for VS Code** — a VS Code extension for building stream processing applications using
Confluent Cloud, Apache Kafka, and Apache Flink. Integrates with Confluent Cloud products and Apache
Kafka-compatible clusters within VS Code.

## Core Commands

```bash
npx gulp build              # Development build
npx gulp check              # TypeScript type checking
npx gulp lint               # ESLint (add -f for auto-fix)
npx gulp test               # Unit tests (Mocha/Sinon)
npx gulp test -t "name"     # Run specific test(s) by name
npx gulp functional          # Webview tests (Playwright)
npx gulp e2e                # End-to-end tests (Playwright + Electron)
npx gulp e2e -t "name"      # Run specific E2E test(s) by name
npx gulp test --coverage    # Generate Istanbul coverage reports
```

## Golden Rules

1. **Disposable resource management**: ALL event-listening classes MUST extend
   `DisposableCollection` (`src/utils/disposables.ts`). Push every `onDid*` subscription to
   `this.disposables`.
2. **Type safety**: NEVER use `any` type. Pre
```

</details>
