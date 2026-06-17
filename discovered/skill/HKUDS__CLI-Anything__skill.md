---
name: HKUDS__CLI-Anything__skill
source: https://github.com/HKUDS/CLI-Anything/blob/bf3cc39e2edb0be313e395077e4cd3f1f4573c53/hermes-skill/SKILL.md
repo: HKUDS/CLI-Anything
kind: skill
stars: 43092
last_pushed: 2026-06-14T09:27:52Z
license: apache-2.0
score: 8
domains: [cli-tools, agents-ai, automation]
tags: [harness-building, adapter-pattern, json-interfaces]
curated: 2026-06-15
curated_by: config-scout
---

# HKUDS/CLI-Anything — skill

**Why it's worth keeping:** It defines a rigorous architecture for tool-making, including mandatory namespace packaging, machine-readable output requirements, and a specific strategy for wrapping real backends rather than reimplementing them.

**Summary:** Provides instructions for an agent to build 'harnesses'—structured Python CLI wrappers that transform existing software into machine-readable, stateful, and JSON-compatible tools.

**Source credibility:** High; the HKUDS repository is well-starred and focuses on making software 'agent-native'.

**Recency:** Current; utilizes modern Python packaging and tool-calling patterns.

**Source:** [HKUDS/CLI-Anything/hermes-skill/SKILL.md](https://github.com/HKUDS/CLI-Anything/blob/bf3cc39e2edb0be313e395077e4cd3f1f4573c53/hermes-skill/SKILL.md) · 43092★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cli-anything-hermes
description: Use when the user wants Hermes Agent to build, refine, test, or validate a CLI-Anything harness for a GUI application or source repository. Adapts the CLI-Anything methodology to Hermes without changing the generated Python harness format.
---

# CLI-Anything for Hermes Agent

Use this skill when the user wants Hermes Agent to act like the `CLI-Anything` builder.

Before implementation, use the full methodology source of truth when available:

1. If this skill is being used from inside the `CLI-Anything` repository, read `../cli-anything-plugin/HARNESS.md` first.
2. If that local file is unavailable, clone or download `cli-anything-plugin` from `https://github.com/HKUDS/CLI-Anything/tree/main/cli-anything-plugin`, then use `HARNESS.md` and the resources around it from that folder.
3. Only if both local and network retrieval fail, follow the condensed rules below.

## Inputs

Accept either:

- A local source path such as `./gimp` or `/path/to/software`
- A GitHub repository URL

Derive the software name from the local directory name after cloning if needed.

## Hermes Tool Bindings

Hermes agents build harnesses by combining these built-in
```

</details>
