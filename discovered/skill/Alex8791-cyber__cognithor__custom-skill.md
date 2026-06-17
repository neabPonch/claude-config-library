---
name: Alex8791-cyber__cognithor__custom-skill
source: https://github.com/Alex8791-cyber/cognithor/blob/78212af5396fd42cb7103b9edfe9b2e57909aac5/examples/custom_skill.md
repo: Alex8791-cyber/cognithor
kind: skill
stars: 147
last_pushed: 2026-06-08T10:39:19Z
license: apache-2.0
score: 7
domains: [software-engineering, security, devops]
tags: [code-review, quality-assurance, best-practices]
curated: 2026-06-15
curated_by: config-scout
---

# Alex8791-cyber/cognithor — skill

**Why it's worth keeping:** The specific output schema (Critical/Warning/Suggestion) and the 'Known Pitfalls' instruction to avoid accidental file modification are excellent transferable patterns.

**Summary:** Provides a highly structured methodology for conducting code reviews, emphasizing severity levels and specific categories like security and performance.

**Source credibility:** High; part of an active Agent OS project with significant community traction.

**Recency:** Current; aligns well with modern agentic workflows and tool-calling paradigms.

**Source:** [Alex8791-cyber/cognithor/examples/custom_skill.md](https://github.com/Alex8791-cyber/cognithor/blob/78212af5396fd42cb7103b9edfe9b2e57909aac5/examples/custom_skill.md) · 147★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: code-review
trigger_keywords: [Code-Review, Review, Codequalität, Code prüfen, Pull Request]
tools_required: [read_file, list_directory, analyze_code]
category: coding
priority: 5
description: "Performs structured code review on a file or directory"
enabled: true
---
# Code Review

## When to Apply
When the user asks for a code review, quality check, or wants feedback on
their code. Typical triggers: "Review this file", "Check the code quality",
"What can I improve in src/...".

## Prerequisites
- A file path or directory to review
- Optional: specific focus areas (security, performance, readability)

## Steps
1. **Identify target** — Ask which file or directory to review if not specified.
2. **Read the code** — Use `read_file` to load the target. For directories,
   use `list_directory` first, then read key files.
3. **Analyze** — Use `analyze_code` for automated metrics (complexity,
   duplication, style). Note any issues.
4. **Review manually** — Check for:
   - Security: injection, hardcoded credentials, path traversal
   - Performance: unnecessary loops, missing caching, N+1 queries
   - Readability: naming, function length, comments
   - Architecture: coupling, sing
```

</details>
