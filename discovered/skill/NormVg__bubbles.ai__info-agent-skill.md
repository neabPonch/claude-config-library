---
name: NormVg__bubbles.ai__info-agent-skill
source: https://github.com/NormVg/bubbles.ai/blob/47e653463b07f1d4315df626243f7c631ed60e32/.info2ai/info-agent-skill.md
repo: NormVg/bubbles.ai
kind: skill
stars: 0
last_pushed: 2026-04-17T21:57:06Z
license: other
score: 8
domains: [agents-ai, architecture, cli-tools]
tags: [progressive-disclosure, skill-framework, context-management]
curated: 2026-06-16
curated_by: config-scout
---

# NormVg/bubbles.ai — skill

**Why it's worth keeping:** It solves the context-bloat problem by only loading full instructions via a `loadSkill` tool when required; establishes a structured directory pattern for bundling assets, code, and documentation with specific skills.

**Summary:** A technical blueprint for implementing an agentic 'skill' system using progressive disclosure to manage context windows.

**Source credibility:** Low social proof (0 stars) but high technical quality in logic and implementation structure.

**Recency:** Very current; addresses contemporary challenges in long-context agent management.

**Source:** [NormVg/bubbles.ai/.info2ai/info-agent-skill.md](https://github.com/NormVg/bubbles.ai/blob/47e653463b07f1d4315df626243f7c631ed60e32/.info2ai/info-agent-skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Add Skills to Your Agent

In this guide, you will learn how to extend your agent with [Agent Skills](https://agentskills.io), a lightweight, open format for adding specialized knowledge and workflows that load at runtime from markdown files.

At its core, a skill is a folder containing a `SKILL.md` file with metadata and instructions that tell an agent how to perform a specific task.

```
my-skill/
├── SKILL.md          # Required: instructions + metadata
├── scripts/          # Optional: executable code
├── references/       # Optional: documentation
└── assets/           # Optional: templates, resources
```

## How Skills Work

Skills use **progressive disclosure** to manage context efficiently:

1. **Discovery**: At startup, agents load only the name and description of each available skill (just enough to know when it might be relevant)
2. **Activation**: When a task matches a skill's description, the agent reads the full `SKILL.md` instructions into context
3. **Execution**: The agent follows the instructions, optionally loading referenced files or executing bundled code as needed

This approach keeps agents fast while giving them access to more context on demand.

## The SK
```

</details>
