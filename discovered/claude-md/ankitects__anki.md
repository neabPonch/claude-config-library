---
name: ankitects__anki
source: https://github.com/ankitects/anki/blob/8546af7cdf7dced07b4108ff4e2fb8496eb944f9/CLAUDE.md
repo: ankitects/anki
kind: claude-md
stars: 28548
last_pushed: 2026-06-14T20:20:37Z
license: other
score: 9
domains: [multi-language, rust, python, web-frontend]
tags: [architecture, build-system, workflow, ipc]
curated: 2026-06-15
curated_by: config-scout
---

# ankitects/anki — claude-md

**Why it's worth keeping:** Mandates using 'just' as a single source of truth for all tasks to prevent manual script errors; includes specific language-specific iteration/test patterns.

**Summary:** Provides a highly structured guide to Anki's multi-language architecture, focusing on the interactions between Rust, Python, and TypeScript.

**Source credibility:** Extremely high; Anki is a major, highly active open-source project.

**Recency:** Very current; utilizes modern tooling like 'just', Svelte, and Rust workspaces.

**Source:** [ankitects/anki/CLAUDE.md](https://github.com/ankitects/anki/blob/8546af7cdf7dced07b4108ff4e2fb8496eb944f9/CLAUDE.md) · 28548★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Configuration

> **Note:** Every command you need — building, running, testing, linting,
> formatting — is defined as a recipe in the project `justfile`. Run
> `just --list` to see them. Do not invoke `./ninja`, `./run`, or scripts
> under `./tools` directly — use the `just` recipes instead.

## Project Overview

Anki is a spaced repetition flashcard program with a multi-layered architecture. Main components:

- Web frontend: Svelte/TypeScript in ts/
- PyQt GUI, which embeds the web components in aqt/
- Python library which wraps our rust Layer (pylib/, with Rust module in pylib/rsbridge)
- Core Rust layer in rslib/
- Protobuf definitions in proto/ that are used by the different layers to
  talk to each other.

## Running Anki

To build and run Anki in development mode:

```
just run
```

This builds pylib and qt, then launches Anki with debugging enabled. Web
views are served at http://localhost:40000/_anki/pages/ (e.g.,
deckconfig.html). Use `just run-optimized` for a release-optimized build.
For live-reloading during web development, run `just web-watch` in a
separate terminal — it monitors ts/, sass/, and qt/aqt/data/web/ and
auto-rebuilds on changes (`just rebuil
```

</details>
