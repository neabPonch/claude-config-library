---
name: flashbots__builder-playground__skill
source: https://github.com/flashbots/builder-playground/blob/e5d8e7610891ec08f558c93d6bc069a1af589058/docs/SKILL.md
repo: flashbots/builder-playground
kind: skill
stars: 131
last_pushed: 2026-06-16T05:05:30Z
license: mit
score: 8
domains: [blockchain, cli-tools, devops]
tags: [protocol-rules, environment-config]
curated: 2026-06-16
curated_by: config-scout
---

# flashbots/builder-playground — skill

**Why it's worth keeping:** Demonstrates high-value techniques such as strict execution sequencing, specific domain-knowledge mapping (consensus client flags), and guardrails against context bloat and unintended parallelization.

**Summary:** Detailed operational protocols for an agent to manage a blockchain builder environment via the `builder-playground` CLI.

**Source credibility:** High; maintained by Flashbots, a leading entity in Ethereum infrastructure development.

**Recency:** Current; utilizes sophisticated grounding and tool-use strategies highly applicable to modern Claude Code workflows.

**Source:** [flashbots/builder-playground/docs/SKILL.md](https://github.com/flashbots/builder-playground/blob/e5d8e7610891ec08f558c93d6bc069a1af589058/docs/SKILL.md) · 131★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
@custom_recipes.md
@custom_recipes_guide.md

# Rules and suggestions

These suggestions apply everywhere including outside of this section.

Refrain from reading the builder-playground codebase directly to avoid context bloat and long thinking cycles.

If there is an ambiguity about how to solve a specific problem about any of the service software and it requires delving deep, state the problem back to the user and prompt to choose a direction. While going in the chosen direction, prefer smaller steps in reasoning and solving.

Stick to the most optimistic and the fastest path while figuring out the details and working on the implementations. Save troubleshooting to the debugging phase.

Do not run exploratory commands to resolve further ambiguity. Ask the user immediately if you have understood the potential problem solving direction to continue with, well enough.

If you notice that you are going in circles while thinking after two iterations, prompt the user with a few directions unless stated otherwise by the user.

Never parallelize recipe generation and file reads - work on each item sequentially.

You already have `builder-playground` installed in the host system. Verify wit
```

</details>
