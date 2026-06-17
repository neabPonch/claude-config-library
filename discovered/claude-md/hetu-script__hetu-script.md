---
name: hetu-script__hetu-script
source: https://github.com/hetu-script/hetu-script/blob/3d1a8705fd1b5036db3c67cb72f5bdc1ed5ef895/CLAUDE.md
repo: hetu-script/hetu-script
kind: claude-md
stars: 272
last_pushed: 2026-05-15T07:55:33Z
license: mit
score: 9
domains: [compiler-design, language-implementation, dart-flutter, monorepo]
tags: [monorepo, build-automation, architecture-patterns, language-engine]
curated: 2026-06-14
curated_by: config-scout
---

# hetu-script/hetu-script — claude-md

**Why it's worth keeping:** The inclusion of a 'Compiler Pipeline' diagram, specific language syntax gotchas (Dart switch cases), and clear tables mapping package responsibilities are highly transferable techniques.

**Summary:** This file provides an excellent structural map of a complex compiler monorepo including architectural patterns and build workflows.

**Source credibility:** The repository shows active maintenance and significant community interest with 270+ stars.

**Recency:** Current; includes modern Dart-specific technical nuances.

**Source:** [hetu-script/hetu-script/CLAUDE.md](https://github.com/hetu-script/hetu-script/blob/3d1a8705fd1b5036db3c67cb72f5bdc1ed5ef895/CLAUDE.md) · 272★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# About Dart

Remember: In mordern Dart, non-empty case clauses jump to the end of the switch after completion. They do not require a break statement.

# AI Agent Instructions — Hetu Script

## Project Overview

Hetu Script is a lightweight scripting language written in Dart, designed for embedding in Flutter apps. It runs on all Flutter-supported platforms.

- **Website**: https://hetu.dev
- **Docs (EN)**: https://hetu.dev/docs/en-US/
- **Online playground**: https://hetu.dev/codepad/

## Monorepo Structure

| Package                 | Path                              | Purpose                                                                            |
| ----------------------- | --------------------------------- | ---------------------------------------------------------------------------------- |
| `hetu_script`           | `packages/hetu_script/`           | Core language implementation (lexer, parser, AST, analyzer, compiler, interpreter) |
| `hetu_script_dev_tools` | `packages/hetu_script_dev_tools/` | CLI REPL tool and file system integration                                          |
| `hetu_script_flutter`   | `packages/hetu_script_flutter/`   | Flutter asset loading via
```

</details>
