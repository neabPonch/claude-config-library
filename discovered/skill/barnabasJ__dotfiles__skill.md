---
name: barnabasJ__dotfiles__skill
source: https://github.com/barnabasJ/dotfiles/blob/f866ea4da20a0069fd8083ec61c1f49db0506a78/agents/skills/elixir-docs/SKILL.md
repo: barnabasJ/dotfiles
kind: skill
stars: 3
last_pushed: 2026-05-05T19:12:23Z
license: unknown
score: 9
domains: [backend, elixir]
tags: [documentation-protocol, search-hierarchy, dependency-inspection]
curated: 2026-06-15
curated_by: config-scout
---

# barnabasJ/dotfiles — skill

**Why it's worth keeping:** The 'hierarchy of truth' approach prevents API hallucinations by teaching the agent to treat local `deps/` as the primary source of truth using specific Grep and file-path patterns.

**Summary:** An expert-level documentation lookup protocol that prioritizes local dependency inspection over web searches to ensure version accuracy.

**Source credibility:** Low star count, but content demonstrates high domain expertise in Elixir toolchains.

**Recency:** Very current; includes modern MCP integration and standard Elixir development workflows.

**Source:** [barnabasJ/dotfiles/agents/skills/elixir-docs/SKILL.md](https://github.com/barnabasJ/dotfiles/blob/f866ea4da20a0069fd8083ec61c1f49db0506a78/agents/skills/elixir-docs/SKILL.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: elixir-docs
description: Elixir documentation search and lookup
---

# Elixir Documentation Search

Systematic approach to finding Elixir documentation and answers. Follow this
hierarchy from most authoritative to least.

## Search Hierarchy

**Always follow this order - stop when you find the answer:**

1. **Local deps folder** - Source code and docs in `deps/`
2. **Tidewave MCP** - If available, use for live documentation
3. **mix usage_rules** - Project-specific documentation
4. **HexDocs websearch** - Official package documentation
5. **Elixir Forum / DeepWiki** - Community knowledge
6. **General websearch** - Last resort

## 1. Local Deps Folder (First Choice)

**The most authoritative source - actual source code the project uses:**

```bash
# Find the module in deps
deps/<package_name>/lib/

# Examples:
deps/phoenix/lib/phoenix/controller.ex
deps/ecto/lib/ecto/query.ex
deps/ash/lib/ash/resource.ex
```

### Search Strategies

**Find a module:**

```elixir
# Module Phoenix.Controller is at:
deps/phoenix/lib/phoenix/controller.ex

# Module Ash.Resource is at:
deps/ash/lib/ash/resource.ex
```

**Search for a function:**

```bash
# Use Grep tool to find function definiti
```

</details>
