---
name: EveryInc__compound-engineering-plugin__skill
source: https://github.com/EveryInc/compound-engineering-plugin/blob/3437de3049ea975bceec2688940d696e16cc5f87/plugins/compound-engineering/skills/ce-plan/SKILL.md
repo: EveryInc/compound-engineering-plugin
kind: skill
stars: 21420
last_pushed: 2026-06-15T17:26:21Z
license: mit
score: 9
domains: [software-engineering, ai-agents, cli-tools]
tags: [technical-planning, architecture, workflow-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# EveryInc/compound-engineering-plugin — skill

**Why it's worth keeping:** It utilizes a sophisticated 'Design vs. Implementation' philosophy, mandates repo-relative paths for portability, and includes complex configuration resolution logic.

**Summary:** This skill transforms high-level ideas into rigorous technical design documents by enforcing strict boundaries between planning and execution.

**Source credibility:** High; the 21k+ stars on the source repository demonstrate significant community trust and proven utility.

**Recency:** Very current; it integrates deeply with Claude Code's specific tool-calling patterns like AskUserQuestion/ToolSearch.

**Source:** [EveryInc/compound-engineering-plugin/plugins/compound-engineering/skills/ce-plan/SKILL.md](https://github.com/EveryInc/compound-engineering-plugin/blob/3437de3049ea975bceec2688940d696e16cc5f87/plugins/compound-engineering/skills/ce-plan/SKILL.md) · 21420★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ce-plan
description: "Create structured plans for multi-step tasks -- software features, research workflows, events, study plans, or any goal that benefits from breakdown. Also deepens existing plans with interactive sub-agent review. Use when the user says 'plan this', 'create a plan', 'how should we build', 'break this down', or when a brainstorm doc is ready for planning. Use 'deepen the plan' or 'deepening pass' for the deepening flow. For exploratory requests, prefer ce-brainstorm first."
argument-hint: "[optional: feature description, requirements doc path, plan path to deepen, or any task to plan] [output:html]"
---

# Create Technical Plan

**Note: The current year is 2026.** Use this when dating plans and searching for recent documentation.

`ce-brainstorm` defines **WHAT** to build. `ce-plan` defines **HOW** to build it. `ce-work` executes the plan. A prior brainstorm is useful context but never required — `ce-plan` works from any input: a requirements doc, a bug report, a feature idea, or a rough description.

**When directly invoked, always plan.** Never classify a direct invocation as "not a planning task" and abandon the workflow. If the input is unclear, as
```

</details>
