---
name: parcadei__Continuous-Claude-v3__skill
source: https://github.com/parcadei/Continuous-Claude-v3/blob/d07ff4b06b62f43771bc0c927d0211b734d6149e/.claude/skills/help/SKILL.md
repo: parcadei/Continuous-Claude-v3
kind: skill
stars: 3813
last_pushed: 2026-01-26T15:27:49Z
license: mit
score: 9
domains: [agents-ai, cli-tools, devops]
tags: [orchestration, workflow, discovery]
curated: 2026-06-15
curated_by: config-scout
---

# parcadei/Continuous-Claude-v3 — skill

**Why it's worth keeping:** Demonstrates powerful patterns for token-efficient codebase exploration (tldr) and structured multi-agent role definitions to manage complex task lifecycles.

**Summary:** Acts as a command center for an agentic orchestration framework, mapping out high-level workflows, specialized sub-agents, and system hooks.

**Source credibility:** High; highly starred repository indicating a mature framework for context management.

**Recency:** Current; aligns with modern agentic orchestration and tool-use patterns.

**Source:** [parcadei/Continuous-Claude-v3/.claude/skills/help/SKILL.md](https://github.com/parcadei/Continuous-Claude-v3/blob/d07ff4b06b62f43771bc0c927d0211b734d6149e/.claude/skills/help/SKILL.md) · 3813★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: help
description: Interactive workspace discovery - learn what tools, workflows, agents, and hooks are available
triggers: ["help", "what can you do", "show capabilities", "how do I"]
allowed-tools: [AskUserQuestion, Bash, Read, Glob, Grep]
priority: high
---

# /help - Workspace Discovery

Guide users through the capabilities of this workspace setup.

## Usage

```
/help                    # Interactive guided discovery
/help workflows          # Workflow orchestration skills
/help agents             # Specialist agents catalog
/help tools              # CLI tools (tldr, prove, recall)
/help hooks              # Active hooks and what they do
/help advanced           # MCP, frontmatter, customization
/help <name>             # Deep dive on specific skill/agent
```

## Behavior Based on Arguments

### No Arguments: Interactive Discovery

Use AskUserQuestion to guide the user:

```
question: "What are you trying to do?"
header: "Goal"
options:
  - label: "Explore/understand a codebase"
    description: "Find patterns, architecture, conventions"
  - label: "Fix a bug"
    description: "Investigate, diagnose, implement fix"
  - label: "Build a feature"
    description: "Plan,
```

</details>
