---
name: ithinkihaveacat__dotfiles__jetpack-skill
source: https://github.com/ithinkihaveacat/dotfiles/blob/6fe8ef7b1d25b8d1b2a8e6e3f0aec21d98e5041d/prompts/jetpack-skill.md
repo: ithinkihaveacat/dotfiles
kind: skill
stars: 47
last_pushed: 2026-06-16T16:57:41Z
license: apache-2.0
score: 9
domains: [agents-ai, cli-tools, devops]
tags: [skill-specification, agent-instructions, blueprint]
curated: 2026-06-16
curated_by: config-scout
---

# ithinkihaveacat/dotfiles — skill

**Why it's worth keeping:** It codifies advanced patterns like 'Script First' command prioritization, optimized frontmatter constraints, and explicit discovery via trigger phrases to prevent tool ambiguity.

**Summary:** A high-fidelity specification and blueprint for creating professional-grade Agent Skills.

**Source credibility:** The highly structured requirement set suggests a deep understanding of agentic system prompts and tool-call discovery logic.

**Recency:** Extremely current; aligns with modern LLM-driven agent/tool interaction standards.

**Source:** [ithinkihaveacat/dotfiles/prompts/jetpack-skill.md](https://github.com/ithinkihaveacat/dotfiles/blob/6fe8ef7b1d25b8d1b2a8e6e3f0aec21d98e5041d/prompts/jetpack-skill.md) · 47★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Prompt: Create Jetpack Library Utilities Skill

Create an Agent Skill that helps agents work with Android Jetpack libraries.
This skill should document the `jetpack` script's capabilities and strongly
encourage agents to use the script over raw commands.

## Goal

Produce a self-contained skill directory at `skills/jetpack/` that an agent can
use to:

1. Run the bundled `jetpack` script directly (fast, deterministic, with
   intelligent package resolution, search, and version handling)
2. Only fall back to raw commands when the script fails due to missing
   dependencies

**Important:** The `jetpack` script provides significant value beyond raw
commands (e.g., package-to-coordinate resolution with exceptions table, code
search, version type handling, Kotlin Multiplatform support). The skill must
make agents prefer the script by default and only consult raw commands as a last
resort by reading the script source.

## Research Phase

Before creating files, research the following:

1. **Review the Agent Skills specification** at
   <https://agentskills.io/specification.md> to understand frontmatter
   requirements, directory structure, and naming conventions.

2. **Examine `skills/je
```

</details>
