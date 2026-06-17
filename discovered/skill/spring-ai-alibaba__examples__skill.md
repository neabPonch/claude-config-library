---
name: spring-ai-alibaba__examples__skill
source: https://github.com/spring-ai-alibaba/examples/blob/996af804d1c106702c5fe728e33cb743f794925f/.claude/skills/readme-generate/SKILL.md
repo: spring-ai-alibaba/examples
kind: skill
stars: 2730
last_pushed: 2026-06-06T04:20:17Z
license: apache-2.0
score: 8
domains: [backend-api, documentation, cli-tools]
tags: [readme-generation, spring-boot, automation]
curated: 2026-06-15
curated_by: config-scout
---

# spring-ai-alibaba/examples — skill

**Why it's worth keeping:** Demonstrates the 'Analysis-then-Generation' pattern where a specialized script performs deep structural analysis to ensure documentation accuracy that LLMs alone might miss.

**Summary:** An automation skill that generates comprehensive, structured README.md files by analyzing Spring Boot module source code and configurations.

**Source credibility:** High; part of a highly starred, actively maintained Spring AI ecosystem repository.

**Recency:** 

**Source:** [spring-ai-alibaba/examples/.claude/skills/readme-generate/SKILL.md](https://github.com/spring-ai-alibaba/examples/blob/996af804d1c106702c5fe728e33cb743f794925f/.claude/skills/readme-generate/SKILL.md) · 2730★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: readme-generate
description: Generates comprehensive README.md files for Spring Boot modules based on task specification requirements
---

# README Generator

This skill automatically analyzes Spring Boot modules and generates comprehensive README.md files according to the specified format requirements, including module functionality, API documentation, usage examples, technical implementation, testing guidance, and important notes.

## When to Use

Use this skill when you need to:

- Generate README.md files for new modules
- Update existing README.md files when module content changes
- Create consistent documentation across multiple modules
- Document API interfaces automatically
- Provide comprehensive module documentation for developers

## How to Use

### Generate README for a Module

Execute the README generator script to create comprehensive documentation:

```bash
python .claude/skills/readme-generate/scripts/readme_generator.py <module_path> [output_file]
```

**Parameters:**
- `module_path` (required): Path to the Spring Boot module directory
- `output_file` (optional): Custom output file path (default: `{module_path}/README.md`)

**Examples:**
```bash
# Generat
```

</details>
