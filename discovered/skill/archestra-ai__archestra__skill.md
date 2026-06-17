---
name: archestra-ai__archestra__skill
source: https://github.com/archestra-ai/archestra/blob/38e896167f1cb8079987ed1892c8cb74244a8f0e/migration-kit/SKILL.md
repo: archestra-ai/archestra
kind: skill
stars: 3834
last_pushed: 2026-06-15T02:16:04Z
license: agpl-3.0
score: 9
domains: [agents-ai, cli-tools, devops, migration]
tags: [migration, orchestration, enterprise, automation]
curated: 2026-06-15
curated_by: config-scout
---

# archestra-ai/archestra — skill

**Why it's worth keeping:** It utilizes a 'Spine' architecture (deterministic scripts + LLM reasoning), includes a critical path-rewriting step for sandboxing, and implements strict security protocols for secret handling.

**Summary:** A sophisticated migration skill that orchestrates a multi-step deterministic workflow using zero-dependency Python helpers and LLM judgment to port local agentic setups to the Archestra platform.

**Source credibility:** High; part of an enterprise AI platform with significant popularity and recent maintenance.

**Recency:** Very current; specifically designed to handle modern agentic artifacts like MCP and Claude Code configurations.

**Source:** [archestra-ai/archestra/migration-kit/SKILL.md](https://github.com/archestra-ai/archestra/blob/38e896167f1cb8079987ed1892c8cb74244a8f0e/migration-kit/SKILL.md) · 3834★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: migrate-to-archestra
description: Migrate an existing agentic PoC/pilot (Claude Code project files, MCP configs, hooks, local tools, openclaw config, or similar hand-rolled setup artifacts) into an Archestra instance. Use when the user wants to move, port, or convert an existing agentic setup into an Archestra pilot.
license: Apache-2.0
---

# Migrate an agentic PoC to Archestra

You migrate a user's existing agentic PoC or pilot into Archestra. The skill itself runs in Claude
Code, but the source setup may be a messy mix of Claude Code-style files, MCP config, local scripts,
hooks, openclaw config, and other pilot artifacts. The mechanical, deterministic work lives in
bundled Python helpers; you own the product judgment: mapping decisions, asking the user where
ambiguous, getting approval on a preview, and writing the final report.

`$SKILL_DIR` below is the directory containing this file. The helpers are at `$SKILL_DIR/scripts/`.
They are **zero-dependency** and target **Python ≥3.10**, so on a stock interpreter (no `uv`, no
`pip install`, no network) `python3 "$SKILL_DIR/scripts/<x>.py"` just works — important for locked-down
or air-gapped enterprise hosts. `uv run "$S
```

</details>
