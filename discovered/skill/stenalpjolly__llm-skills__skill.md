---
name: stenalpjolly__llm-skills__skill
source: https://github.com/stenalpjolly/llm-skills/blob/b20b2ace3a423e6fd6f405cee2354e965de32a9c/skills/detecting-llm-laziness-and-duplicates/SKILL.md
repo: stenalpjolly/llm-skills
kind: skill
stars: 3
last_pushed: 2026-06-13T14:01:17Z
license: unknown
score: 8
domains: [cli-tools, code-quality, devops]
tags: [automation, refactoring, agentic-patterns]
curated: 2026-06-14
curated_by: config-scout
---

# stenalpjolly/llm-skills — skill

**Why it's worth keeping:** It demonstrates a highly transferable architectural pattern: using cheap, local heuristics to generate a report that the LLM then uses for surgical, high-context analysis.

**Summary:** Uses a 'Quality Control Oracle' (QCO) pattern to detect LLM-generated stubs and duplicates via a local Python scan rather than full-file reading.

**Source credibility:** Low social proof (3 stars), but the technical sophistication of the proposed workflow suggests it's a well-thought-out expert tool.

**Recency:** Very current; specifically addresses the context window and token cost constraints inherent in modern agentic workflows.

**Source:** [stenalpjolly/llm-skills/skills/detecting-llm-laziness-and-duplicates/SKILL.md](https://github.com/stenalpjolly/llm-skills/blob/b20b2ace3a423e6fd6f405cee2354e965de32a9c/skills/detecting-llm-laziness-and-duplicates/SKILL.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: detecting-llm-laziness-and-duplicates
description: >-
  Identifies LLM-generated duplicate code, TODO/FIXME comments, static/lazy stubs, mock data, and placeholder files in a codebase. Use when reviewing recent LLM-generated PRs or commits, analyzing build failures due to omitted/lazy ellipses, or auditing codebases for structural duplicates. Don't use for generic dependency updates, linting formatting style, or refactoring unrelated clean code.
---

# Detecting LLM Laziness and Duplicates

This skill provides a structured method to detect and resolve common LLM coding defects—such as code duplication, TODO comments, static placeholder stubs, and lazy code truncations (e.g., `// ... rest of code stays the same`).

To scan large repositories without overflowing the LLM's context window, this skill employs a **QCO (Quality Control Oracle)** mechanism. Instead of reading all files into the LLM, a local python scanner extracts suspect snippets, which the LLM then analyzes selectively.

## Core Rules

1. **Verify via Local Parser First**: Do not read random codebase files to hunt for laziness. Run the local QCO parser script (`python3 scripts/detect_laziness_and_duplicates.py`
```

</details>
