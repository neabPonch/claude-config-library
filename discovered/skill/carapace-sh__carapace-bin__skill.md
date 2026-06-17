---
name: carapace-sh__carapace-bin__skill
source: https://github.com/carapace-sh/carapace-bin/blob/4cf6531bcd32f4df63d4e3218361d3f980340dfb/skills/carapace/SKILL.md
repo: carapace-sh/carapace-bin
kind: skill
stars: 1857
last_pushed: 2026-06-14T19:52:31Z
license: mit
score: 9
domains: [cli-tools, shell]
tags: [indexing, context-management, documentation-routing]
curated: 2026-06-15
curated_by: config-scout
---

# carapace-sh/carapace-bin — skill

**Why it's worth keeping:** Employs a 'hub-and-spoke' context strategy, enabling efficient, granular information retrieval without overwhelming the context window with irrelevant details.

**Summary:** Acts as a high-level documentation hub that routes agents to specialized sub-references based on task keywords.

**Source credibility:** High; Carapace is a well-starred, highly-maintained tool for shell completion.

**Recency:** Very recent; repo shows activity within the last month.

**Source:** [carapace-sh/carapace-bin/skills/carapace/SKILL.md](https://github.com/carapace-sh/carapace-bin/blob/4cf6531bcd32f4df63d4e3218361d3f980340dfb/skills/carapace/SKILL.md) · 1857★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: carapace
description: >
  Use when working with carapace shell completion — integrating into CLIs, writing YAML specs,
  creating custom actions, looking up macros, setting up shell completion, configuring
  choices/bridges, using the MCP server, or adding man page documentation.
user-invocable: true
---

# Carapace Usage Reference

Reference for using [carapace](https://carapace.sh) shell completion — integrating into CLIs, writing specs, creating actions, and configuring completions.

## Sub-Resources

Load the reference that matches your task. When in doubt, load multiple references.

| Keywords | Reference |
|----------|----------|
| Integrate carapace, cobra, PreRun, PreInvoke, bridge, standalone mode, flag config, non-POSIX flags | [references/integrate.md](references/integrate.md) |
| Custom actions, ActionValues, ActionCallback, ActionExecCommand, modifiers, naming, caching, batch, MultiParts, UID, tags | [references/action.md](references/action.md) |
| YAML spec, user spec, flags, subcommands, parsing modes, completion, macros, modifiers, runnable specs | [references/spec.md](references/spec.md) |
| Macro format, MacroN, MacroI, MacroV, $files, macro signatures,
```

</details>
