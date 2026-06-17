---
name: openai__skills__skill
source: https://github.com/openai/skills/blob/a8924c2a35cfa290458852c4fad17c9133054c2e/skills/.curated/figma-code-connect-components/SKILL.md
repo: openai/skills
kind: skill
stars: 22165
last_pushed: 2026-05-29T16:20:41Z
license: unknown
score: 9
domains: [web-frontend, design-to-code, cli-tools]
tags: [figma, code-connect, workflow-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# openai/skills — skill

**Why it's worth keeping:** It provides highly specific 'agentic' instructions: exact data transformation logic (hyphen-to-colon conversion), search heuristics for finding matching components in a codebase, and clear human-in-the-loop interaction patterns.

**Summary:** Orchestrates the mapping of Figma design components to local code implementations using Figma's Code Connect feature.

**Source credibility:** High structural quality; the template demonstrates advanced prompt engineering techniques used in high-end tool orchestration.

**Recency:** Highly relevant to modern designer-developer handoff workflows and contemporary agentic tool-use requirements.

**Source:** [openai/skills/skills/.curated/figma-code-connect-components/SKILL.md](https://github.com/openai/skills/blob/a8924c2a35cfa290458852c4fad17c9133054c2e/skills/.curated/figma-code-connect-components/SKILL.md) · 22165★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: figma-code-connect-components
description: Connects Figma design components to code components using Code Connect mapping tools. Use when user says "code connect", "connect this component to code", "map this component", "link component to code", "create code connect mapping", or wants to establish mappings between Figma designs and code implementations. For canvas writes via `use_figma`, use `figma-use`.
---

# Code Connect Components

## Overview

This skill helps you connect Figma design components to their corresponding code implementations using Figma's Code Connect feature. It analyzes the Figma design structure, searches your codebase for matching components, and establishes mappings that maintain design-code consistency.

## Skill Boundaries

- Use this skill for `get_code_connect_suggestions` + `send_code_connect_mappings` workflows.
- If the task requires writing to the Figma canvas with Plugin API scripts, switch to [figma-use](../figma-use/SKILL.md).
- If the task is building or updating a full-page screen in Figma from code or a description, switch to [figma-generate-design](../figma-generate-design/SKILL.md).
- If the task is implementing product code from Fi
```

</details>
