---
name: ReyemTech__skills__teardown-skill
source: https://github.com/ReyemTech/skills/blob/08f8f7121f029efea0cc7f0acd12e78dd7b1cc20/teardown.skill.md
repo: ReyemTech/skills
kind: skill
stars: 0
last_pushed: 2026-04-14T17:39:36Z
license: unknown
score: 7
domains: [web-intelligence, reverse-engineering, agents-ai]
tags: [reconnaissance, architecture, sub-agent]
curated: 2026-06-17
curated_by: config-scout
---

# ReyemTech/skills — skill

**Why it's worth keeping:** Uses the Task() pattern to offload heavy investigative workflows into sub-agents, preventing main context pollution. Provides a highly structured, multi-phase lifecycle for intelligence gathering.

**Summary:** Automates web architecture reconnaissance by dispatching a specialized agent to uncover APIs, headers, and third-party services.

**Source credibility:** Low; 0 stars and unknown license suggest a personal or niche repository.

**Recency:** Current; utilizes the Task() pattern relevant to modern Claude Code workflows.

**Source:** [ReyemTech/skills/teardown.skill.md](https://github.com/ReyemTech/skills/blob/08f8f7121f029efea0cc7f0acd12e78dd7b1cc20/teardown.skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: teardown
description: Reverse-engineer any web app's architecture from its frontend. Dispatches to the teardown agent to keep main context clean.
disable-model-invocation: true
allowed-tools: Task
---

# Teardown -- Frontend Architecture Reverse Engineering

When the user invokes `/teardown`, spawn the `teardown` agent via Task() with the user's arguments.

## Usage

```
/teardown <url>
/teardown <url> --name codalio
/teardown <url> --output-dir path/to/output
/teardown <url> --name codalio --output-dir path/to/output
```

## Arguments

- `<url>` (required): Target site to analyze
- `--name <name>` (optional): Short name for the output file
- `--output-dir <path>` (optional): Directory to save results (defaults to `references/intelligence/`)

## Execution

Use Task() to run the `teardown` agent with the user's full arguments. The agent handles all phases:

1. HTTP headers reconnaissance
2. HTML source & JS bundle analysis
3. API discovery (REST, GraphQL, WordPress)
4. Analytics & third-party service identification
5. Compile and save results to the output directory

Wait for the agent to complete and return a summary of findings to the user.
```

</details>
