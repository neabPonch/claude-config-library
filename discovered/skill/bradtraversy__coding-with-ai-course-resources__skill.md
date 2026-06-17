---
name: bradtraversy__coding-with-ai-course-resources__skill
source: https://github.com/bradtraversy/coding-with-ai-course-resources/blob/5f68dd09689f4c1590e92790af7e5d5a3c537ebe/skills/research/SKILL.md
repo: bradtraversy/coding-with-ai-course-resources
kind: skill
stars: 244
last_pushed: 2026-03-15T13:12:06Z
license: mit
score: 7
domains: [documentation, cli-tools]
tags: [research, sop, orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# bradtraversy/coding-with-ai-course-resources — skill

**Why it's worth keeping:** Implements a manifest-driven pattern where task parameters are decoupled from the command, enabling repeatable and highly specific documentation workflows.

**Summary:** Automates technical research by driving execution through external markdown instruction files.

**Source credibility:** The source is an established coding educator with significant social proof via star count.

**Recency:** Very recent; aligns with current agentic tool-use patterns.

**Source:** [bradtraversy/coding-with-ai-course-resources/skills/research/SKILL.md](https://github.com/bradtraversy/coding-with-ai-course-resources/blob/5f68dd09689f4c1590e92790af7e5d5a3c537ebe/skills/research/SKILL.md) · 244★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: research
description: Run a research task to generate documentation
argument-hint: <prompt-name>
---

## Task

Execute research task: $ARGUMENTS

---

### Instructions

1. If no argument provided, error: "Usage: /research <prompt-name>"
2. Look for prompt file at `context/research/{$ARGUMENTS}.md`
3. If not found, error: "Prompt file not found at context/research/{$ARGUMENTS}.md"
4. Read the prompt file which should contain:
   - **Output**: Where to write results (e.g., `context/content-types.md`)
   - **Research**: What to investigate
   - **Include**: Specific details to capture
   - **Sources**: What files/tools to use
5. Execute the research using appropriate tools:
   - Read files (Prisma schema, constants, components)
   - Query database via Neon MCP if needed
   - Search codebase for patterns
6. Write findings to the specified output location
7. Summarize what was discovered

---

### Rules

- This command produces DOCUMENTATION only
- Do NOT modify source code files
- Do NOT create branches or commits
- Output should go to `/docs/` unless otherwise specified
- Use subagents for thorough exploration if needed
```

</details>
